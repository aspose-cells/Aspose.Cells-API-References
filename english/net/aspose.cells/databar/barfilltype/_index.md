---
title: DataBar.BarFillType
second_title: Aspose.Cells for .NET API Reference
description: DataBar property. Gets or sets how a data bar is filled with color
type: docs
url: /net/aspose.cells/databar/barfilltype/
---
## DataBar.BarFillType property

Gets or sets how a data bar is filled with color.

```csharp
public DataBarFillType BarFillType { get; set; }
```

### Examples

```csharp
// Called: dataBar.BarFillType = DataBarFillType.Solid;
public static void DataBar_Property_BarFillType()
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
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(120);
            worksheet.Cells["A3"].PutValue(260);

            // Save the workbook
            workbook.Save("NegativeBarFormatExample.xlsx");
        }
```

### See Also

* enum [DataBarFillType](../../databarfilltype/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


