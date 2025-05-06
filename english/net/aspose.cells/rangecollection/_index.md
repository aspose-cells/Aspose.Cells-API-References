---
title: Class RangeCollection
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.RangeCollection class. Encapsulates a collection of Range objects
type: docs
url: /net/aspose.cells/rangecollection/
---
## RangeCollection class

Encapsulates a collection of [`Range`](../range/) objects.

```csharp
public class RangeCollection : CollectionBase<Range>
```

## Properties

| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/rangecollection/item/) { get; } | Gets the [`Range`](../range/) element at the specified index. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.cells/rangecollection/add/)(Range) | Adds a [`Range`](../range/) item to the collection. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Range) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Range, IComparer&lt;Range&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Range, IComparer&lt;Range&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Range) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Range[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Range[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Range[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Range&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Range&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Range&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Range&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Range&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Range&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Range&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Range&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Range&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Range&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Range) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Range, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Range, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Range) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Range, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Range, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Examples

```csharp
// Called: public static void equals(RangeCollection arrRangeSrc, RangeCollection arrRangeDest, string info)
public static void Type_RangeCollection(RangeCollection arrRangeSrc, RangeCollection arrRangeDest, string info)
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
                        Type_RangeCollection(rangeSrc, rangeDest, info + &quot;.Range&quot; + &quot;[&quot; + i +&quot;]&quot;);
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

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Range](../range/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


