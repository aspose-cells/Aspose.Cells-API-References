---
title: Cells.DeleteColumn
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Deletes a column
type: docs
url: /net/aspose.cells/cells/deletecolumn/
---
## DeleteColumn(int, bool) {#deletecolumn_1}

Deletes a column.

```csharp
public void DeleteColumn(int columnIndex, bool updateReference)
```

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Index of the column to be deleted. |
| updateReference | Boolean | Indicates whether update references in other worksheets. |

### Examples

```csharp
// Called: wb.Worksheets[0].Cells.DeleteColumn(0, true);
[Test]
        public void Method_Boolean_()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "CellsNet46003.xlsx");
            wb.Worksheets.AddCopy(0);
            wb.Worksheets[1].Name = "Copy";
            wb.Worksheets[0].Cells.InsertRows(8, 1, true);
            wb.Worksheets[0].Cells[8, 0].Value = "8";
            wb.Worksheets[0].Cells[8, 1].Value = "Eight";
            wb.Worksheets[0].Cells[8, 2].Value = "Eight - 8";
            wb.Worksheets[0].Cells.DeleteColumn(0, true);
            Shape shape = wb.Worksheets[0].Shapes[0];
            Assert.AreEqual(shape.InputRange, "B$4:B$11");
            shape = wb.Worksheets[1].Shapes[0];
            Assert.AreEqual(shape.InputRange, "C$4:C$10");
            wb.Save(Constants.destPath + "CellsNet46003.xlsx");
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteColumn(int) {#deletecolumn}

Deletes a column.

```csharp
public void DeleteColumn(int columnIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Index of the column to be deleted. |

### Examples

```csharp
// Called: cells.DeleteColumn(0);
[Test]
        public void Method_Int32_()
        {
            caseName = "testDeleteStyle_008";
            Workbook workbook = new Workbook();
          workbook = new Workbook(Constants.sourcePath + "insertDelete\\testStyle.xls");
            Cells cells = workbook.Worksheets[0].Cells;
            cells.DeleteColumn(0);

            checkDeleteStyle_008(workbook);
            workbook.Save(Constants.destPath + "testDeleteStyle.xls");
            workbook = new Workbook(Constants.destPath + "testDeleteStyle.xls");
            checkDeleteStyle_008(workbook);
            workbook.Save(Constants.destPath + "testDeleteStyle.xlsx");
            workbook = new Workbook(Constants.destPath + "testDeleteStyle.xlsx");
            checkDeleteStyle_008(workbook);
            workbook.Save(Constants.destPath + "testDeleteStyle.xml", SaveFormat.SpreadsheetML);
            workbook = new Workbook(Constants.destPath + "testDeleteStyle.xml");
            checkDeleteStyle_008(workbook);
            workbook.Save(Constants.destPath + "testDeleteStyle.xls");
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


