---
title: Range.GetCellOrNull
second_title: Aspose.Cells for .NET API Reference
description: Range method. Gets Cell object or null in this range
type: docs
url: /net/aspose.cells/range/getcellornull/
---
## Range.GetCellOrNull method

Gets [`Cell`](../../cell/) object or null in this range.

```csharp
public Cell GetCellOrNull(int rowOffset, int columnOffset)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | Int32 | Row offset in this range, zero based. |
| columnOffset | Int32 | Column offset in this range, zero based. |

### Return Value

[`Cell`](../../cell/) object.

### Examples

```csharp
// Called: Cell c2 = dest.GetCellOrNull(i, j);
public static void Range_Method_GetCellOrNull(Aspose.Cells.Range source, Aspose.Cells.Range dest,bool checkStyle)
        {
            Assert.AreEqual(source.ColumnCount, dest.ColumnCount);
            Assert.AreEqual(source.RowCount, dest.RowCount);

            int rowCount = source.RowCount;
            int colCount = source.ColumnCount;
            for (int i = 0; i < rowCount; i++)
            {
                for (int j = 0; j < colCount; j++)
                {
                    Cell c1 = source.GetCellOrNull(i, j);
                    Cell c2 = dest.GetCellOrNull(i, j);
                    CompareCell(c1, c2, checkStyle);
                }
            }
        }
```

### See Also

* class [Cell](../../cell/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


