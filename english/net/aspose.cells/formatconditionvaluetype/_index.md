---
title: Enum FormatConditionValueType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.FormatConditionValueType enum. Condition value type
type: docs
url: /net/aspose.cells/formatconditionvaluetype/
---
## FormatConditionValueType enumeration

Condition value type.

```csharp
public enum FormatConditionValueType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Formula | `0` | The minimum/ midpoint / maximum value for the gradient is determined by a formula. |
| Max | `1` | Indicates that the maximum value in the range shall be used as the maximum value for the gradient. |
| Min | `2` | Indicates that the minimum value in the range shall be used as the minimum value for the gradient. |
| Number | `3` | Indicates that the minimum / midpoint / maximum value for the gradient is specified by a constant numeric value. |
| Percent | `4` | Value indicates a percentage between the minimum and maximum values in the range shall be used as the minimum / midpoint / maximum value for the gradient. |
| Percentile | `5` | Value indicates a percentile ranking in the range shall be used as the minimum / midpoint / maximum value for the gradient. |
| AutomaticMax | `6` | Indicates that the Automatic maximum value in the range shall be used as the Automatic maximum value for the gradient. |
| AutomaticMin | `7` | Indicates that the Automatic minimum value in the range shall be used as the Automatic minimum value for the gradient. |

### Examples

```csharp
// Called: fc.ColorScale.MaxCfvo.Type = FormatConditionValueType.Max;
public static void Type_FormatConditionValueType()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Adds an empty conditional formatting
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Sets the conditional format range
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Adds condition
            int conditionIndex = fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[conditionIndex];

            // Setting properties for ColorScale
            fc.ColorScale.Is3ColorScale = true;

            // Setting min value
            fc.ColorScale.MinCfvo.Type = FormatConditionValueType.Min;
            fc.ColorScale.MinCfvo.Value = null;
            fc.ColorScale.MinColor = Color.Blue;

            // Setting mid value
            fc.ColorScale.MidCfvo.Type = FormatConditionValueType.Percentile;
            fc.ColorScale.MidCfvo.Value = 50;
            fc.ColorScale.MidColor = Color.Yellow;

            // Setting max value
            fc.ColorScale.MaxCfvo.Type = FormatConditionValueType.Max;
            fc.ColorScale.MaxCfvo.Value = null;
            fc.ColorScale.MaxColor = Color.Red;

            // Save the workbook
            workbook.Save(&quot;ConditionalFormattingValueExample.xlsx&quot;);
            workbook.Save(&quot;ConditionalFormattingValueExample.pdf&quot;);
            return;
        }
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


