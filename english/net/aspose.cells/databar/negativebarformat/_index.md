---
title: DataBar.NegativeBarFormat
second_title: Aspose.Cells for .NET API Reference
description: DataBar property. Gets the NegativeBarFormat object associated with a data bar conditional formatting rule
type: docs
url: /net/aspose.cells/databar/negativebarformat/
---
## DataBar.NegativeBarFormat property

Gets the NegativeBarFormat object associated with a data bar conditional formatting rule.

```csharp
public NegativeBarFormat NegativeBarFormat { get; }
```

### Examples

```csharp
// Called: NegativeBarFormat negativeBarFormat = dataBar.NegativeBarFormat;
public static void Property_NegativeBarFormat()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data
            worksheet.Cells[&quot;A1&quot;].PutValue(10);
            worksheet.Cells[&quot;A2&quot;].PutValue(-20);
            worksheet.Cells[&quot;A3&quot;].PutValue(30);
            worksheet.Cells[&quot;A4&quot;].PutValue(-40);
            worksheet.Cells[&quot;A5&quot;].PutValue(50);

            // Add conditional formatting
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea ca = new CellArea { StartRow = 0, EndRow = 4, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcs[conditionIndex];

            // Set the data bar properties
            DataBar dataBar = fc.DataBar;
            dataBar.MinCfvo.Type = FormatConditionValueType.Number;
            dataBar.MinCfvo.Value = -50;
            dataBar.MaxCfvo.Type = FormatConditionValueType.Number;
            dataBar.MaxCfvo.Value = 50;
            dataBar.Color = System.Drawing.Color.Green;

            // Set negative bar format properties
            NegativeBarFormat negativeBarFormat = dataBar.NegativeBarFormat;
            negativeBarFormat.Color = System.Drawing.Color.Red;
            negativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            negativeBarFormat.BorderColor = System.Drawing.Color.Blue;
            negativeBarFormat.BorderColorType = DataBarNegativeColorType.SameAsPositive;

            // Save the workbook
            workbook.Save(&quot;DataBarNegativeColorTypeExample.xlsx&quot;);
            workbook.Save(&quot;DataBarNegativeColorTypeExample.pdf&quot;);
            return;
        }
```

### See Also

* class [NegativeBarFormat](../../negativebarformat/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


