---
title: VerticalPageBreakCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: VerticalPageBreakCollection property. Gets the VerticalPageBreak element at the specified index
type: docs
url: /net/aspose.cells/verticalpagebreakcollection/item/
---
## VerticalPageBreakCollection indexer (1 of 2)

Gets the [`VerticalPageBreak`](../../verticalpagebreak/) element at the specified index.

```csharp
public VerticalPageBreak this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp
// Called: AssertHelper.AreEqual(vpagebreaksSrc[i], vpagebreaksDest[i], info + &amp;quot;.VPageBreak&amp;quot;);
public static void Property_Int32_(VerticalPageBreakCollection vpagebreaksSrc, VerticalPageBreakCollection vpagebreaksDest, string info)
        {
            if (AssertHelper.checkNull(vpagebreaksSrc, vpagebreaksDest, info))
            {
                return;
            }
            int countSrc = vpagebreaksSrc.Count;
            int countDest = vpagebreaksDest.Count;
            AssertHelper.AreEqual(countSrc, countDest, info + &quot;.Count&quot;);
            for (int i = 0; i &lt; countSrc &amp;&amp; i &lt; countDest; i++)
            {
                AssertHelper.AreEqual(vpagebreaksSrc[i], vpagebreaksDest[i], info + &quot;.VPageBreak&quot;);
            }
        }
```

### See Also

* class [VerticalPageBreak](../../verticalpagebreak/)
* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## VerticalPageBreakCollection indexer (2 of 2)

Gets the [`VerticalPageBreak`](../../verticalpagebreak/) element with the specified cell name.

```csharp
public VerticalPageBreak this[string cellName] { get; }
```

| Parameter | Description |
| --- | --- |
| cellName | Cell name. |

### Return Value

The element with the specified cell name.

### See Also

* class [VerticalPageBreak](../../verticalpagebreak/)
* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


