---
title: DataSorter.Sort
second_title: Aspose.Cells for .NET API Reference
description: DataSorter method. Sorts the data of the area
type: docs
url: /net/aspose.cells/datasorter/sort/
---
## Sort(Cells, int, int, int, int) {#sort_2}

Sorts the data of the area.

```csharp
public int[] Sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cells | Cells | The cells contains the data area. |
| startRow | Int32 | The start row of the area. |
| startColumn | Int32 | The start column of the area. |
| endRow | Int32 | The end row of the area. |
| endColumn | Int32 | The end column of the area. |

### Return Value

the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns. If no rows/columns needs to be moved by this sorting operation, null will be returned.

### Examples

```csharp
// Called: workbook.DataSorter.Sort(workbook.Worksheets[0].Cells, 4, 3, 6, 5);
[Test]
        // Does Aspose.Cells have ability to add sort fields to ListObjects
        // http://www.aspose.com/community/forums/thread/292632.aspx
        public void Method_Int32_()
        {
            Console.WriteLine("Method_Int32_()");
            string infn = path + @"ListObjectSort\ListObjectSort.xlsx";
            string outfn = Constants.destPath + @"ListObjectSort_out.xlsx";

            Workbook workbook = new Workbook(infn);
            workbook.DataSorter.AddKey(5, SortOrder.Ascending);
            workbook.DataSorter.Sort(workbook.Worksheets[0].Cells, 4, 3, 6, 5);
            Assert.LessOrEqual(workbook.Worksheets[0].Cells["F5"].IntValue,
                workbook.Worksheets[0].Cells["F6"].IntValue);
            Assert.LessOrEqual(workbook.Worksheets[0].Cells["F6"].IntValue,
                workbook.Worksheets[0].Cells["F7"].IntValue);
            workbook.Save(outfn, SaveFormat.Xlsx);
        }
```

### See Also

* class [Cells](../../cells/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Sort(Cells, CellArea) {#sort_1}

Sort the data of the area.

```csharp
public int[] Sort(Cells cells, CellArea area)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cells | Cells | The cells contains the data area. |
| area | CellArea | The area needed to sort |

### Return Value

the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns. If no rows/columns needs to be moved by this sorting operation, null will be returned.

### Examples

```csharp
// Called: sorter.Sort(worksheet.Cells, ca);
[Test]
        public void Method_CellArea_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSJAVA42266.xlsx");

            Worksheet worksheet = workbook.Worksheets[0];

            ////Create your cell area 
            CellArea ca = CellArea.CreateCellArea("A4", "G18");

            //Create your sorter 
            DataSorter sorter = workbook.DataSorter;

            //Find the index, since we want to sort by column A, so we should know 
            //the index for sorter 
            int idx = CellsHelper.ColumnNameToIndex("A");

            //Add key in sorter, it will sort in Ascending order 
            sorter.AddKey(idx, SortOrder.Ascending);

            //Perform sort 
            sorter.Sort(worksheet.Cells, ca);

            Assert.AreEqual("C",workbook.Worksheets[0].Cells["F10"].StringValue);
            Util.SaveManCheck(workbook, "Shape", "CELLSJAVA42266.xlsx");
        }
```

### See Also

* class [Cells](../../cells/)
* struct [CellArea](../../cellarea/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Sort() {#sort}

Sort the data in the range.

```csharp
public int[] Sort()
```

### Return Value

the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns. If no rows/columns needs to be moved by this sorting operation, null will be returned.

### Examples

```csharp
// Called: list.AutoFilter.Sorter.Sort();
[Test]
        public void Method_Sort()
        {
            var size = 1;
            var workbook = new Workbook(Constants.sourcePath + "AutoFilter/CellsNet44880.xlsx");
            var worksheet = workbook.Worksheets[0];
            var list = worksheet.ListObjects["table1"];
            var dataRange = list.DataRange;
            worksheet.Cells.DeleteRange(dataRange.FirstRow + size, dataRange.FirstColumn,
                dataRange.FirstRow + dataRange.RowCount - 1, dataRange.ColumnCount, ShiftType.Up);

            list.AutoFilter.Sorter.Sort();
            // Got this meesage in result file. 
            // We found a problem with some content in 'file'. Do you want us to try to recover as much as we can? If you trust the source of this workbook, click Yes. 
            Util.SaveManCheck(workbook, "Shape", "CellsNet44880.xlsx");
        }
```

### See Also

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


