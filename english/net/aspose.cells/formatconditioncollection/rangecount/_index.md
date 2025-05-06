---
title: FormatConditionCollection.RangeCount
second_title: Aspose.Cells for .NET API Reference
description: FormatConditionCollection property. Gets count of conditionally formatted ranges
type: docs
url: /net/aspose.cells/formatconditioncollection/rangecount/
---
## FormatConditionCollection.RangeCount property

Gets count of conditionally formatted ranges.

```csharp
public int RangeCount { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(1, fcs.RangeCount, &amp;quot;sheet.ConditionalFormattings[0].RangeCount&amp;quot;);
private void Property_RangeCount(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[&quot;Sheet2&quot;];
            ConditionalFormattingCollection cfs = sheet.ConditionalFormattings;
            AssertHelper.AreEqual(1, cfs.Count, &quot;ConditionalFormattings.Count&quot;);
            FormatConditionCollection fcs = sheet.ConditionalFormattings[0];
            AssertHelper.AreEqual(1, fcs.Count, &quot;sheet.ConditionalFormattings[0].Count&quot;);
            AssertHelper.AreEqual(1, fcs.RangeCount, &quot;sheet.ConditionalFormattings[0].RangeCount&quot;);
            FormatCondition fc = fcs[0];
            AssertHelper.AreEqual(OperatorType.NotBetween, fc.Operator, &quot;FormatCondition&quot;);
        }
```

### See Also

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


