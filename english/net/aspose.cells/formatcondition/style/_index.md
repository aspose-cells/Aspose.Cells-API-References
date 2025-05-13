---
title: FormatCondition.Style
second_title: Aspose.Cells for .NET API Reference
description: FormatCondition property. Gets or setts style of conditional formatted cell ranges
type: docs
url: /net/aspose.cells/formatcondition/style/
---
## FormatCondition.Style property

Gets or setts style of conditional formatted cell ranges.

```csharp
public Style Style { get; set; }
```

### Examples

```csharp
// Called: fc2.Style.BackgroundColor = System.Drawing.Color.Green;
public static void FormatCondition_Property_Style()
        {
            // Create a new Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add an empty conditional formatting
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Set the conditional format range
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Add a condition with OperatorType.Between
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A1", "100");
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.Yellow;

            // Add another condition with OperatorType.GreaterThan
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "50", null);
            FormatCondition fc2 = fcs[conditionIndex2];
            fc2.Style.BackgroundColor = System.Drawing.Color.Green;

            // Save the workbook
            workbook.Save("OperatorTypeExample.xlsx");

            return;
        }
```

### See Also

* class [Style](../../style/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


