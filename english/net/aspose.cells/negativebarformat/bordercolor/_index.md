---
title: NegativeBarFormat.BorderColor
second_title: Aspose.Cells for .NET API Reference
description: NegativeBarFormat property. Gets or sets a FormatColor object that you can use to specify the border color for negative data bars
type: docs
url: /net/aspose.cells/negativebarformat/bordercolor/
---
## NegativeBarFormat.BorderColor property

Gets or sets a FormatColor object that you can use to specify the border color for negative data bars.

```csharp
public Color BorderColor { get; set; }
```

### Examples

```csharp
// Called: dataBar.NegativeBarFormat.BorderColor = Color.Yellow;
public static void NegativeBarFormat_Property_BorderColor()
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
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(120);
            sheet.Cells["A3"].PutValue(260);

            // Saving the Excel file
            workbook.Save("DataBarFillTypeExample.xlsx");
            workbook.Save("DataBarFillTypeExample.pdf");
        }
```

### See Also

* class [NegativeBarFormat](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


