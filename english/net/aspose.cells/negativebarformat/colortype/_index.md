---
title: NegativeBarFormat.ColorType
second_title: Aspose.Cells for .NET API Reference
description: NegativeBarFormat property. Gets or sets whether to use the same fill color as positive data bars
type: docs
url: /net/aspose.cells/negativebarformat/colortype/
---
## NegativeBarFormat.ColorType property

Gets or sets whether to use the same fill color as positive data bars.

```csharp
public DataBarNegativeColorType ColorType { get; set; }
```

### Examples

```csharp
// Called: negativeBarFormat.ColorType = DataBarNegativeColorType.Color;
public static void Property_ColorType()
        {
            // Instantiate a Workbook object
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Adds an empty conditional formatting
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Sets the conditional format range
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 10
            };
            fcs.AddArea(ca);

            // Adds condition for DataBar
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcs[conditionIndex];

            // Get DataBar and set its properties
            DataBar dataBar = fc.DataBar;
            dataBar.Color = Color.Orange;
            dataBar.BarFillType = DataBarFillType.Solid;
            dataBar.AxisColor = Color.Red;
            dataBar.AxisPosition = DataBarAxisPosition.Midpoint;

            // Configure the NegativeBarFormat properties
            NegativeBarFormat negativeBarFormat = dataBar.NegativeBarFormat;
            negativeBarFormat.Color = Color.White;
            negativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            negativeBarFormat.BorderColor = Color.Yellow;
            negativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;

            // Put some values in the cells
            worksheet.Cells[&quot;A1&quot;].PutValue(10);
            worksheet.Cells[&quot;A2&quot;].PutValue(120);
            worksheet.Cells[&quot;A3&quot;].PutValue(260);

            // Save the workbook
            workbook.Save(&quot;NegativeBarFormatExample.xlsx&quot;);
        }
```

### See Also

* enum [DataBarNegativeColorType](../../databarnegativecolortype/)
* class [NegativeBarFormat](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


