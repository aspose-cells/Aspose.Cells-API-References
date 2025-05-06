---
title: DataBarBorder.Color
second_title: Aspose.Cells for .NET API Reference
description: DataBarBorder property. Gets or sets the borders color of data bars specified by a conditional formatting rule
type: docs
url: /net/aspose.cells/databarborder/color/
---
## DataBarBorder.Color property

Gets or sets the border's color of data bars specified by a conditional formatting rule.

```csharp
public Color Color { get; set; }
```

### Examples

```csharp
// Called: dataBar.BarBorder.Color = Color.Plum;
public static void Property_Color()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();

            // Adding a new worksheet to the Workbook
            Worksheet sheet = workbook.Worksheets[0];

            // Adds an empty conditional formatting
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Sets the conditional format range.
            CellArea ca = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(ca);

            // Adds condition
            int idx = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = fcs[idx];

            // Get Databar
            DataBar dataBar = cond.DataBar;

            // Set Databar properties
            dataBar.Color = Color.Orange;
            dataBar.MinCfvo.Type = FormatConditionValueType.Percentile;
            dataBar.MinCfvo.Value = 30;
            dataBar.ShowValue = false;
            dataBar.BarBorder.Type = DataBarBorderType.Solid;
            dataBar.BarBorder.Color = Color.Plum;
            dataBar.BarFillType = DataBarFillType.Solid;
            dataBar.AxisColor = Color.Red;
            dataBar.AxisPosition = DataBarAxisPosition.Midpoint;
            dataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.Color = Color.White;
            dataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // Put Cell Values
            sheet.Cells[&quot;A1&quot;].PutValue(10);
            sheet.Cells[&quot;A2&quot;].PutValue(120);
            sheet.Cells[&quot;A3&quot;].PutValue(260);

            // Saving the Excel file
            workbook.Save(&quot;DataBarFillTypeExample.xlsx&quot;);
            workbook.Save(&quot;DataBarFillTypeExample.pdf&quot;);
        }
```

### See Also

* class [DataBarBorder](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


