---
title: FormatCondition.Operator
second_title: Aspose.Cells for .NET API Reference
description: FormatCondition property. Gets and sets the conditional format operator type
type: docs
url: /net/aspose.cells/formatcondition/operator/
---
## FormatCondition.Operator property

Gets and sets the conditional format operator type.

```csharp
public OperatorType Operator { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(OperatorType.LessThan, fc.Operator, &amp;quot;FormatCondition&amp;quot;);
private void Property_Operator(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[0];
            ConditionalFormattingCollection cfs = sheet.ConditionalFormattings;
            AssertHelper.AreEqual(1, cfs.Count, &quot;ConditionalFormattings.Count&quot;);
            FormatConditionCollection fcs = sheet.ConditionalFormattings[0];
            AssertHelper.AreEqual(1, fcs.Count, &quot;sheet.ConditionalFormattings[0].Count&quot;);
            AssertHelper.AreEqual(1, fcs.RangeCount, &quot;sheet.ConditionalFormattings[0].RangeCount&quot;);
            FormatCondition fc = fcs[0];
            AssertHelper.AreEqual(OperatorType.LessThan, fc.Operator, &quot;FormatCondition&quot;);
        }
```

### See Also

* enum [OperatorType](../../operatortype/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


