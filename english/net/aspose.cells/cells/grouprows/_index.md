---
title: Cells.GroupRows
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Groups rows
type: docs
url: /net/aspose.cells/cells/grouprows/
---
## GroupRows(int, int, bool) {#grouprows_1}

Groups rows.

```csharp
public void GroupRows(int firstIndex, int lastIndex, bool isHidden)
```

| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | Int32 | The first row index to be grouped. |
| lastIndex | Int32 | The last row index to be grouped. |
| isHidden | Boolean | Specifies if the grouped rows are hidden. |

### Examples

```csharp
// Called: workbook.Worksheets[0].Cells.GroupRows(1, 2, false);
[Test]
        public void Method_Boolean_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "Test_192714.xls");

            workbook.Worksheets[0].Cells.GroupRows(1, 2, false);

            DataSorter dataSorter = workbook.DataSorter;
            dataSorter.HasHeaders = true;

            CellArea ca = new CellArea();

            dataSorter.Key1 = 0;

            dataSorter.Order1 = Aspose.Cells.SortOrder.Descending;

            ca.StartRow = 0;

            ca.StartColumn = 0;

            ca.EndColumn = 1;

            ca.EndRow = 12;

            dataSorter.Sort(workbook.Worksheets[0].Cells, ca);
            Assert.AreEqual(workbook.Worksheets[0].Cells["A10"].StringValue, "1996");

            workbook.Save(Constants.destPath + "Test_192714.xls");
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GroupRows(int, int) {#grouprows}

Groups rows.

```csharp
public void GroupRows(int firstIndex, int lastIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | Int32 | The first row index to be grouped. |
| lastIndex | Int32 | The last row index to be grouped. |

### Examples

```csharp
// Called: cells.GroupRows(-1, 2);
[Test, ExpectedException(typeof(CellsException))]
#endif
        public void Method_Int32_()
        {
            caseName = "testGroupRows_Exception_001";
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells.GroupRows(-1, 2);
            string msg = message + "cells.GroupRows(-1, 2)";
            writeToExcel(caseName, msg);            
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


