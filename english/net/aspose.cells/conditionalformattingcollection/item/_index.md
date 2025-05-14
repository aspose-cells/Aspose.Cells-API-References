---
title: ConditionalFormattingCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ConditionalFormattingCollection property. Gets the FormatConditions element at the specified index
type: docs
url: /net/aspose.cells/conditionalformattingcollection/item/
---
## ConditionalFormattingCollection indexer

Gets the FormatConditions element at the specified index.

```csharp
public FormatConditionCollection this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Examples

```csharp
// Called: FormatConditionCollection fcs = sheet.ConditionalFormattings[0];
private void ConditionalFormattingCollection_Property_Item(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[0];
            ConditionalFormattingCollection cfs = sheet.ConditionalFormattings;
            AssertHelper.AreEqual(1, cfs.Count, "ConditionalFormattings.Count");
            FormatConditionCollection fcs = sheet.ConditionalFormattings[0];
            AssertHelper.AreEqual(1, fcs.Count, "sheet.ConditionalFormattings[0].Count");
            AssertHelper.AreEqual(1, fcs.RangeCount, "sheet.ConditionalFormattings[0].RangeCount");
            FormatCondition fc = fcs[0];
            AssertHelper.AreEqual(OperatorType.Between, fc.Operator, "FormatCondition");
        }
```

### See Also

* class [FormatConditionCollection](../../formatconditioncollection/)
* class [ConditionalFormattingCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


