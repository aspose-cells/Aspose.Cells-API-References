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
// Called: Aspose.Cells.Range rangeDest = arrRangeDest[j];
public static void Property_Int32_(RangeCollection arrRangeSrc, RangeCollection arrRangeDest, string info)
        {
            if (AssertHelper.checkNull(arrRangeSrc, arrRangeDest, info))
            {
                return;
            }
            int countSrc = arrRangeSrc.Count;
            int countDest = arrRangeDest.Count;
            AssertHelper.AreEqual(countSrc, countDest, info + ".Count");         

            for (int i = 0; i < countSrc; i++)
            {
                Aspose.Cells.Range rangeSrc = arrRangeSrc[i];
                bool IsSame = false;
                for (int j = 0; j < countDest; j++)
                {
                    IsSame = false;
                    Aspose.Cells.Range rangeDest = arrRangeDest[j];
                    if (rangeSrc.FirstRow == rangeDest.FirstRow && rangeSrc.FirstColumn == rangeDest.FirstColumn &&
                        rangeSrc.RowCount == rangeDest.RowCount && rangeSrc.ColumnCount == rangeDest.ColumnCount)
                    {
                        Property_Int32_(rangeSrc, rangeDest, info + ".Range" + "[" + i +"]");
                        IsSame = true;
                        break;
                    }
                }
                if (!IsSame)
                {
                    AssertHelper.Fail("Ranges isn't same!");
                }
            }


        }
```

### See Also

* class [Range](../../range/)
* class [RangeCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


