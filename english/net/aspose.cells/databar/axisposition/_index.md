---
title: DataBar.AxisPosition
second_title: Aspose.Cells for .NET API Reference
description: DataBar property. Gets or sets the position of the axis of the data bars specified by a conditional formatting rule
type: docs
url: /net/aspose.cells/databar/axisposition/
---
## DataBar.AxisPosition property

Gets or sets the position of the axis of the data bars specified by a conditional formatting rule.

```csharp
public DataBarAxisPosition AxisPosition { get; set; }
```

### Examples

```csharp
// Called: dataBar.AxisPosition = DataBarAxisPosition.Midpoint;
public static void Property_AxisPosition()
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

* enum [DataBarAxisPosition](../../databaraxisposition/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


