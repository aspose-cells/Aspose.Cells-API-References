---
title: LegendEntryCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: LegendEntryCollection property. Gets the LegendEntry element at the specified index
type: docs
url: /net/aspose.cells.charts/legendentrycollection/item/
---
## LegendEntryCollection indexer

Gets the [`LegendEntry`](../../legendentry/) element at the specified index.

```csharp
public LegendEntry this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp
// Called: LegendEntry legendentrySrc = legendentriesSrc[i];
public static void LegendEntryCollection_Property_Item(LegendEntryCollection legendentriesSrc, LegendEntryCollection legendentriesDest, string info)
        {
            if (AssertHelper.checkNull(legendentriesSrc, legendentriesDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(legendentriesSrc.Count, legendentriesDest.Count, info + ".Count");
            int countSrc = legendentriesSrc.Count;
            int countDest = legendentriesDest.Count;
            for (int i = 0; i < countSrc && i < countDest; i++)
            {
                LegendEntry legendentrySrc = legendentriesSrc[i];
                LegendEntry legendentryDest = legendentriesDest[i];               
                LegendEntryCollection_Property_Item(legendentriesSrc[i], legendentriesDest[i], info+".LegendEntry"+"[" + i + "]");
            }
        }
```

### See Also

* class [LegendEntry](../../legendentry/)
* class [LegendEntryCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


