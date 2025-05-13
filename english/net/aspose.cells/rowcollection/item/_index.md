---
title: RowCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: RowCollection property. Gets a Row object by given row index. The Row object of given row index will be instantiated if it does not exist before
type: docs
url: /net/aspose.cells/rowcollection/item/
---
## RowCollection indexer

Gets a [`Row`](../../row/) object by given row index. The Row object of given row index will be instantiated if it does not exist before.

```csharp
public Row this[int rowIndex] { get; }
```

### Examples

```csharp
// Called: Row row = cells.Rows[i];
private Workbook RowCollection_Property_Item()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            cells.StandardWidth = 40.0;
            for (int i = 0; i < 10; i++)
            {
                Row row = cells.Rows[i];
                StyleProcessRow(row, true, null);
                StyleProcessCell(row[i], true, null);
            }
            return wb;
        }
```

### See Also

* class [Row](../../row/)
* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


