---
title: FormatCondition.Type
second_title: Aspose.Cells for .NET API Reference
description: FormatCondition property. Gets and sets whether the conditional format Type
type: docs
url: /net/aspose.cells/formatcondition/type/
---
## FormatCondition.Type property

Gets and sets whether the conditional format Type.

```csharp
public FormatConditionType Type { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(FormatConditionType.Expression, fc.Type, "sheet.ConditionalFormattings[0]" + "[" + i + "].Type");
private void FormatCondition_Property_Type(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[0];
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

* enum [FormatConditionType](../../formatconditiontype/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


