---
title: Worksheet.ConditionalFormattings
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets the ConditionalFormattings in the worksheet
type: docs
url: /net/aspose.cells/worksheet/conditionalformattings/
---
## Worksheet.ConditionalFormattings property

Gets the ConditionalFormattings in the worksheet.

```csharp
public ConditionalFormattingCollection ConditionalFormattings { get; }
```

### Examples

```csharp
// Called: ConditionalFormattingCollection cfs = sheet.ConditionalFormattings;
private void Worksheet_Property_ConditionalFormattings(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets["Sheet5"];
            ConditionalFormattingCollection cfs = sheet.ConditionalFormattings;
            AssertHelper.AreEqual(1, cfs.Count, "ConditionalFormattings.Count");
            FormatConditionCollection fcs = sheet.ConditionalFormattings[0];
            AssertHelper.AreEqual(1, fcs.Count, "sheet.ConditionalFormattings[0].Count");
            AssertHelper.AreEqual(1, fcs.RangeCount, "sheet.ConditionalFormattings[0].RangeCount");
            FormatCondition fc = fcs[0];
            AssertHelper.AreEqual(OperatorType.GreaterThan, fc.Operator, "FormatCondition");
        }
```

### See Also

* class [ConditionalFormattingCollection](../../conditionalformattingcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


