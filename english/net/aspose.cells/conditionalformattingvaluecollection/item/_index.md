---
title: ConditionalFormattingValueCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ConditionalFormattingValueCollection property. Get the CFValueObject element at the specified index
type: docs
url: /net/aspose.cells/conditionalformattingvaluecollection/item/
---
## ConditionalFormattingValueCollection indexer

Get the CFValueObject element at the specified index.

```csharp
public ConditionalFormattingValue this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp
// Called: equals(arrcfoSrc[i], arrcfoDest[i], info);
public static void ConditionalFormattingValueCollection_Property_Item(ConditionalFormattingValueCollection arrcfoSrc, ConditionalFormattingValueCollection arrcfoDest, string info)
        {
            if (AssertHelper.checkNull(arrcfoSrc, arrcfoDest, info))
            {
                return;
            }
            int countSrc = arrcfoSrc.Count;
            int countDest = arrcfoDest.Count;
            AssertHelper.AreEqual(countSrc, countDest, info + ".Count");
            for (int i = 0; i < countSrc && i < countDest; i++)
            {
                ConditionalFormattingValueCollection_Property_Item(arrcfoSrc[i], arrcfoDest[i], info);
            }

        }
```

### See Also

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [ConditionalFormattingValueCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


