---
title: FormatConditionCollection.Count
second_title: Aspose.Cells for .NET API Reference
description: FormatConditionCollection property. Gets the count of the conditions
type: docs
url: /net/aspose.cells/formatconditioncollection/count/
---
## FormatConditionCollection.Count property

Gets the count of the conditions.

```csharp
public int Count { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(2, fcs.Count, "sheet.ConditionalFormattings[0].Count");
private void Property_Count(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets["Sheet2"];
            ConditionalFormattingCollection cfs = sheet.ConditionalFormattings;
            AssertHelper.AreEqual(1, cfs.Count, "ConditionalFormattings.Count");
            FormatConditionCollection fcs = sheet.ConditionalFormattings[0];
            AssertHelper.AreEqual(2, fcs.Count, "sheet.ConditionalFormattings[0].Count");
            AssertHelper.AreEqual(2, fcs.RangeCount, "sheet.ConditionalFormattings[0].RangeCount");
            for (int i = 0; i < fcs.Count; i++)
            {
                FormatCondition fc = fcs[i];
                AssertHelper.AreEqual(FormatConditionType.Expression, fc.Type, "sheet.ConditionalFormattings[0]" + "[" + i + "].Type");
            }
        }
```

### See Also

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


