---
title: Cells.DeleteRows
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Deletes multiple rows
type: docs
url: /net/aspose.cells/cells/deleterows/
---
## DeleteRows(int, int) {#deleterows}

Deletes multiple rows.

```csharp
public bool DeleteRows(int rowIndex, int totalRows)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | The first row index to be deleted. |
| totalRows | Int32 | Count of rows to be deleted. |

### Remarks

If the deleted range contains the top part(not whole) of the table(ListObject), the ranged could not be deleted and nothing will be done. It works in the same way with MS Excel.

### Examples

```csharp
// Called: cells.DeleteRows(1, 3);
[Test]
        public void Method_Int32_()
        {
            caseName = "testDeleteRows_004";
            Workbook workbook = new Workbook(Constants.sourcePath + "Cells\\deleteColumn_002.xls");
            Cells cells = workbook.Worksheets[0].Cells;
            cells.DeleteRows(1, 3);

            checkDeleteRows_004(workbook);
            workbook.Save(Constants.destPath + "testDeleteRows.xls");
            workbook = new Workbook(Constants.destPath + "testDeleteRows.xls");
            checkDeleteRows_004(workbook);
            workbook.Save(Constants.destPath + "testDeleteRows.xlsx");
            workbook = new Workbook(Constants.destPath + "testDeleteRows.xlsx");
            checkDeleteRows_004(workbook);
            workbook.Save(Constants.destPath + "testDeleteRows.xml", SaveFormat.SpreadsheetML);
            workbook = new Workbook(Constants.destPath + "testDeleteRows.xml");
            checkDeleteRows_004(workbook);
            workbook.Save(Constants.destPath + "testDeleteRows.xls");
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteRows(int, int, bool) {#deleterows_2}

Deletes multiple rows in the worksheet.

```csharp
public bool DeleteRows(int rowIndex, int totalRows, bool updateReference)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Index of the first row to be deleted. |
| totalRows | Int32 | Count of rows to be deleted. |
| updateReference | Boolean | Indicates whether update references in other worksheets. |

### Examples

```csharp
// Called: workbook.Worksheets[1].Cells.DeleteRows(6, 20, false);
[Test]
        public void Method_Boolean_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSJAVA41108.xlsx");
            workbook.Worksheets[1].Cells.DeleteRows(6, 20, false);
            Assert.AreEqual(workbook.Worksheets[1].Cells["J7"].GetStyle().Font.Color.B, 255);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteRows(int, int, DeleteOptions) {#deleterows_1}

Deletes multiple rows in the worksheet.

```csharp
public bool DeleteRows(int rowIndex, int totalRows, DeleteOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Index of the first row to be deleted. |
| totalRows | Int32 | Count of rows to be deleted. |
| options | DeleteOptions | Options for the deleting operation |

### Examples

```csharp
// Called: cells.DeleteRows(2, 1, new DeleteOptions() { FormulaChangeMonitor = monitor });
[Test]
        public void Method_DeleteOptions_()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            cells[0, 0].Formula = "=A5";
            sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[0];
            fcc.Add(CellArea.CreateCellArea(0, 3, 1, 4), FormatConditionType.Expression,
                OperatorType.Equal, "=A8>0", "");
            FormulaChangeMonitorSimple monitor = new FormulaChangeMonitorSimple(wb);
            cells.DeleteRows(2, 1, new DeleteOptions() { FormulaChangeMonitor = monitor });
            Assert.AreEqual("0-0-0", monitor.mChangedCell, "Changed cell");
            Assert.AreEqual("0-0-0", monitor.mFormatCondition, "Changed format condition");
        }
```

### See Also

* class [DeleteOptions](../../deleteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


