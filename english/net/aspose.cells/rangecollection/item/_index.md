---
title: RangeCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: RangeCollection property. Gets the Range element at the specified index
type: docs
url: /net/aspose.cells/rangecollection/item/
---
## RangeCollection indexer

Gets the [`Range`](../../range/) element at the specified index.

```csharp
public Range this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp
// Called: Aspose.Cells.Range rangeSrc = arrRangeSrc[i];
public static void Property_Int32_(RangeCollection arrRangeSrc, RangeCollection arrRangeDest, string info)
        {
            if (AssertHelper.checkNull(arrRangeSrc, arrRangeDest, info))
            {
                return;
            }
            int countSrc = arrRangeSrc.Count;
            int countDest = arrRangeDest.Count;
            AssertHelper.AreEqual(countSrc, countDest, info + &quot;.Count&quot;);         

            for (int i = 0; i &lt; countSrc; i++)
            {
                Aspose.Cells.Range rangeSrc = arrRangeSrc[i];
                bool IsSame = false;
                for (int j = 0; j &lt; countDest; j++)
                {
                    IsSame = false;
                    Aspose.Cells.Range rangeDest = arrRangeDest[j];
                    if (rangeSrc.FirstRow == rangeDest.FirstRow &amp;&amp; rangeSrc.FirstColumn == rangeDest.FirstColumn &amp;&amp;
                        rangeSrc.RowCount == rangeDest.RowCount &amp;&amp; rangeSrc.ColumnCount == rangeDest.ColumnCount)
                    {
                        Property_Int32_(rangeSrc, rangeDest, info + &quot;.Range&quot; + &quot;[&quot; + i +&quot;]&quot;);
                        IsSame = true;
                        break;
                    }
                }
                if (!IsSame)
                {
                    AssertHelper.Fail(&quot;Ranges isn&apos;t same!&quot;);
                }
            }


        }
```

### See Also

* class [Range](../../range/)
* class [RangeCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


