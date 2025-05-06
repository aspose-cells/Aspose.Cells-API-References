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
// Called: checkRowStyle(cells.Rows[7].GetStyle());
private void Property_Int32_(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            checkStyle(cells[3, 1].GetStyle());
            testAreEqual(false, cells[3, 2].IsStyleSet, caseName);
            checkStyle(cells[4, 2].GetStyle());
            checkStyle(cells[4, 3].GetStyle());
            checkStyle(cells[5, 2].GetStyle());
            checkStyle(cells[5, 3].GetStyle());
            checkRowStyle(cells.Rows[7].GetStyle());
            checkColumnStyle(cells[0, 5].GetStyle());
            checkColumnStyle(cells[1, 5].GetStyle());
            testAreEqual(false, cells[2, 5].IsStyleSet, caseName);
            testAreEqual(false, cells[3, 5].IsStyleSet, caseName);
            checkColumnStyle(cells[2, 3].GetStyle());
            checkColumnStyle(cells[3, 3].GetStyle());
            for (int row = 4; row &lt;= 6; row++)
            {
                checkColumnStyle(cells[row, 5].GetStyle());
            }
            checkColumnStyle(cells[99, 5].GetStyle());
            checkColumnStyle(cells[187, 5].GetStyle());
            checkColumnStyle(cells[872, 5].GetStyle());
            checkColumnStyle(cells[1201, 5].GetStyle());
            checkColumnStyle(cells[9721, 5].GetStyle());
            checkColumnStyle(cells[21302, 5].GetStyle());
            checkColumnStyle(cells[65534, 5].GetStyle());
            checkColumnStyle(cells[65535, 5].GetStyle());
        }
```

### See Also

* class [Row](../../row/)
* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


