---
title: HorizontalPageBreakCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: HorizontalPageBreakCollection property. Gets the HorizontalPageBreak element at the specified index
type: docs
url: /net/aspose.cells/horizontalpagebreakcollection/item/
---
## HorizontalPageBreakCollection indexer (1 of 2)

Gets the [`HorizontalPageBreak`](../../horizontalpagebreak/) element at the specified index.

```csharp
public HorizontalPageBreak this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp
// Called: AssertHelper.AreEqual(hpagebreaksSrc[i], hpagebreaksDest[i], info + &amp;quot;.HPageBreak&amp;quot;);
public static void Property_Int32_(HorizontalPageBreakCollection hpagebreaksSrc, HorizontalPageBreakCollection hpagebreaksDest, string info)
        {
            if (AssertHelper.checkNull(hpagebreaksSrc, hpagebreaksDest, info))
            {
                return;
            }
            int countSrc = hpagebreaksSrc.Count;
            int countDest = hpagebreaksDest.Count;
            AssertHelper.AreEqual(countSrc, countDest, info + &quot;.Count&quot;);
            for (int i = 0; i &lt; countSrc &amp;&amp; i &lt; countDest; i++)
            {
                AssertHelper.AreEqual(hpagebreaksSrc[i], hpagebreaksDest[i], info + &quot;.HPageBreak&quot;);
            }
        }
```

### See Also

* class [HorizontalPageBreak](../../horizontalpagebreak/)
* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## HorizontalPageBreakCollection indexer (2 of 2)

Gets the [`HorizontalPageBreak`](../../horizontalpagebreak/) element with the specified cell name.

```csharp
public HorizontalPageBreak this[string cellName] { get; }
```

| Parameter | Description |
| --- | --- |
| cellName | Cell name. |

### Return Value

The element with the specified cell name.

### See Also

* class [HorizontalPageBreak](../../horizontalpagebreak/)
* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


