---
title: ColumnCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ColumnCollection property. Gets a Column object by column index. The Column object of given column index will be instantiated if it does not exist before
type: docs
url: /net/aspose.cells/columncollection/item/
---
## ColumnCollection indexer

Gets a [`Column`](../../column/) object by column index. The Column object of given column index will be instantiated if it does not exist before.

```csharp
public Column this[int columnIndex] { get; }
```

### Examples

```csharp
// Called: checkColumnStyle(cells.Columns[5].GetStyle());
private void Property_Int32_(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            checkRangeStyle(cells);
            checkRowStyle(cells[7, 0].GetStyle());
            checkRowStyle(cells[7, 1].GetStyle());
            checkRowStyle(cells[7, 2].GetStyle());
            checkRowStyle(cells[7, 3].GetStyle());
            checkRowStyle(cells[7, 4].GetStyle());
            checkRowStyle(cells[9, 5].GetStyle());
            checkRowStyle(cells[7, 6].GetStyle());
            checkRowStyle(cells[7, 7].GetStyle());
            checkRowStyle(cells[7, 92].GetStyle());
            checkRowStyle(cells[7, 186].GetStyle());
            checkRowStyle(cells[7, 229].GetStyle());
            checkRowStyle(cells[7, 254].GetStyle());
            checkRowStyle(cells[7, 255].GetStyle());
            checkColumnStyle(cells.Columns[5].GetStyle());
        }
```

### See Also

* class [Column](../../column/)
* class [ColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


