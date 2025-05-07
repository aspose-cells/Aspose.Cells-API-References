---
title: DataSorter.Order3
second_title: Aspose.Cells for .NET API Reference
description: DataSorter property. Represents sort order of the third key
type: docs
url: /net/aspose.cells/datasorter/order3/
---
## DataSorter.Order3 property

Represents sort order of the third key.

```csharp
public SortOrder Order3 { get; set; }
```

### Examples

```csharp
// Called: sorter.Order3 = SortOrder.Ascending;
[Test]
        public void Property_Order3()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            cells[0, 0].PutValue(3);
            cells[1, 0].PutValue(1);
            cells[2, 0].PutValue(2);
            cells[3, 1].PutValue(5);
            cells[4, 1].PutValue(4);
            cells[5, 1].PutValue(6);
            cells[6, 2].PutValue(7);
            cells[7, 2].PutValue(9);
            cells[8, 2].PutValue(8);
            DataSorter sorter = wb.DataSorter;
            sorter.Order1 = SortOrder.Ascending;
            sorter.Key1 = 0; // sort by first data column

            sorter.Order2 = SortOrder.Ascending;
            sorter.Key2 = 1; // then by second data column

            sorter.Order3 = SortOrder.Ascending;
            sorter.Key3 = 2; // then by third data column

            sorter.Sort(cells, CellArea.CreateCellArea(0, 0, 8, 2));
            for (int i = 0; i < 9; i++)
            {
                Assert.AreEqual(i + 1, cells[i, i / 3].IntValue, "Row-" + i);
            }
        }
```

### See Also

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


