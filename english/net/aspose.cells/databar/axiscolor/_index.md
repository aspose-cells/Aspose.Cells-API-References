---
title: DataBar.AxisColor
second_title: Aspose.Cells for .NET API Reference
description: DataBar property. Gets the color of the axis for cells with conditional formatting as data bars
type: docs
url: /net/aspose.cells/databar/axiscolor/
---
## DataBar.AxisColor property

Gets the color of the axis for cells with conditional formatting as data bars.

```csharp
public Color AxisColor { get; set; }
```

### Examples

```csharp
// Called: dataBar.AxisColor = Color.Red;
public static void Property_AxisColor()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();
            
            // Accessing the first worksheet in the workbook
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Adding a conditional formatting rule
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Setting the conditional format range
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);
            
            // Adding a data bar condition
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcs[conditionIndex];
            DataBar dataBar = fc.DataBar;
            
            // Setting properties for the data bar
            dataBar.Color = Color.Orange;
            dataBar.MinCfvo.Type = FormatConditionValueType.Percentile;
            dataBar.MinCfvo.Value = 30;
            dataBar.ShowValue = false;
            dataBar.BarBorder.Type = DataBarBorderType.Solid;
            dataBar.BarBorder.Color = Color.Plum;
            dataBar.BarFillType = DataBarFillType.Solid;
            dataBar.AxisColor = Color.Red;
            dataBar.AxisPosition = DataBarAxisPosition.Midpoint; // Using DataBarAxisPosition enum
            dataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.Color = Color.White;
            dataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.BorderColor = Color.Yellow;
            
            // Putting cell values
            worksheet.Cells[&quot;A1&quot;].PutValue(10);
            worksheet.Cells[&quot;A2&quot;].PutValue(120);
            worksheet.Cells[&quot;A3&quot;].PutValue(260);
            
            // Saving the Excel file
            workbook.Save(&quot;DataBarAxisPositionExample.xlsx&quot;);
            workbook.Save(&quot;DataBarAxisPositionExample.pdf&quot;);
        }
```

### See Also

* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


