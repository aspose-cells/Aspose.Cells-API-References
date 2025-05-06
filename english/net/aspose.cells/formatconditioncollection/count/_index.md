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
// Called: AssertHelper.AreEqual(1, fcs.Count, &amp;quot;sheet.ConditionalFormattings[0].Count&amp;quot;);
private void Property_Count(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[&quot;Sheet8&quot;];
            ConditionalFormattingCollection cfs = sheet.ConditionalFormattings;
            AssertHelper.AreEqual(1, cfs.Count, &quot;ConditionalFormattings.Count&quot;);
            FormatConditionCollection fcs = sheet.ConditionalFormattings[0];
            AssertHelper.AreEqual(1, fcs.Count, &quot;sheet.ConditionalFormattings[0].Count&quot;);
            AssertHelper.AreEqual(1, fcs.RangeCount, &quot;sheet.ConditionalFormattings[0].RangeCount&quot;);
            FormatCondition fc = fcs[0];
            AssertHelper.AreEqual(OperatorType.LessOrEqual, fc.Operator, &quot;FormatCondition&quot;);
        }
```

### See Also

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


