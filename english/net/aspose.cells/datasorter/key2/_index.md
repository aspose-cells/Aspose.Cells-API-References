---
title: DataSorter.Key2
second_title: Aspose.Cells for .NET API Reference
description: DataSorter property. Represents second sorted column indexabsolute position column A is 0 B is 1 
type: docs
url: /net/aspose.cells/datasorter/key2/
---
## DataSorter.Key2 property

Represents second sorted column index(absolute position, column A is 0, B is 1, ...).

```csharp
public int Key2 { get; set; }
```

### Examples

```csharp
// Called: sorter.Key2 = 1;
[Test]
        public void Property_Key2()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            int[] vs = new int[] { 1, 3, 2, 6, 4, 5, 8, 9, 7 };
            for (int i = 0; i < vs.Length; i++)
            {
                cells[i, i / 3].PutValue(vs[i]);
            }
            DataSorter sorter = wb.DataSorter;
            sorter.Clear();
            sorter.Order1 = SortOrder.Ascending;
            sorter.Key1 = 2;
            sorter.Order2 = SortOrder.Ascending;
            sorter.Key2 = 1;
            sorter.Order3 = SortOrder.Ascending;
            sorter.Key3 = 0;
            sorter.Sort(cells, CellArea.CreateCellArea(0, 0, 8, 2));
            vs = new int[] { 7, 8, 9, 4, 5, 6, 1, 2, 3 };
            for (int i = 0; i < vs.Length; i++)
            {
                Cell cell = cells[i, 2 - i / 3];
                Assert.AreEqual(vs[i], cell.IntValue, cell.Name);
            }
        }
```

### See Also

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


