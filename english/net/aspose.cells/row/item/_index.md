---
title: Row.Item
second_title: Aspose.Cells for .NET API Reference
description: Row property. Gets the cell
type: docs
url: /net/aspose.cells/row/item/
---
## Row indexer

Gets the cell.

```csharp
public Cell this[int column] { get; }
```

| Parameter | Description |
| --- | --- |
| column | The column index |

### Examples

```csharp
// Called: cell = row[i];
[Test]
        public void Property_Int32_()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            Style style = wb.CreateStyle();
            style.Font.Size = 16;
            Cell cell;
            cell = cells[0, 0];
            cell.PutValue(3);
            cell.SetStyle(style);
            cell = cells[1, 0];
            cell.PutValue(2);
            cell.SetStyle(style);
            cell = cells[3, 0];
            cell.PutValue(0);
            cell.SetStyle(style);
            cell = cells[2, 0];
            cell.PutValue(1);
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thick, Color.Red);
            cell.SetStyle(style);
            DataSorter sorter = wb.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);
            sorter.CaseSensitive = false;
            sorter.HasHeaders = false;
            sorter.Sort(cells, CellArea.CreateCellArea(0, 0, 3, 1));
            for(int i=0; i&lt;4; i++)
            {
                cell = cells[i, 0];
                style = cell.GetStyle();
                Assert.AreEqual(i, cell.IntValue, &quot;Sorted value of row &quot; + i);
                Assert.AreEqual(16, style.Font.Size, &quot;FontSize of row &quot; + i);
                Assert.AreEqual(i == 2 ? CellBorderType.Thick : CellBorderType.None,
                    style.Borders[BorderType.BottomBorder].LineStyle,
                    &quot;SortRows should not move border togather with data: row &quot; + i);
            }
            Row row = cells.Rows[0];
            cell = row[1];
            cell.PutValue(4);
            cell.SetStyle(style);
            cell = row[2];
            cell.PutValue(3);
            cell.SetStyle(style);
            cell = row[4];
            cell.PutValue(1);
            cell.SetStyle(style);
            cell = row[3];
            cell.PutValue(2);
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thick, Color.Red);
            cell.SetStyle(style);
            sorter.SortLeftToRight = true;
            sorter.Sort(cells, CellArea.CreateCellArea(0, 1, 0, 4));
            //Currently we do not support to keep borders at the original position, should be same with sorting rows.
            for (int i = 1; i &lt; -5; i++)
            {
                cell = row[i];
                Assert.AreEqual(i, cell.IntValue, &quot;Sorted value of col &quot; + i);
                style = cell.GetStyle();
                Assert.AreEqual(16, style.Font.Size, &quot;FontSize of col &quot; + i);
                Assert.AreEqual(i == 3 ? CellBorderType.Thick : CellBorderType.None,
                    style.Borders[BorderType.BottomBorder].LineStyle,
                    &quot;SortCols should not move border togather with data: col &quot; + i);
            }
        }
```

### See Also

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


