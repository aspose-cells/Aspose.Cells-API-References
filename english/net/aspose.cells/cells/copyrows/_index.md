---
title: Cells.CopyRows
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Copies data and formats of some whole rows
type: docs
url: /net/aspose.cells/cells/copyrows/
---
## CopyRows(Cells, int, int, int) {#copyrows}

Copies data and formats of some whole rows.

```csharp
public void CopyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells | Cells | Source Cells object contains data and formats to copy. |
| sourceRowIndex | Int32 | Source row index. |
| destinationRowIndex | Int32 | Destination row index. |
| rowNumber | Int32 | The copied row number. |

### Examples

```csharp
// Called: cellsDest.CopyRows(cellsSrc, 0, 0, 43);
[Test, Ignore("Not ready to test this yet")]
        public void Method_Int32_()
        {
            caseName = "testCopyRows_Shape_001";
            Workbook workbook = new Workbook();            
            workbook = new Workbook(Constants.sourcePath + "Copy//testShape.xls");
            Worksheet sheetSrc = workbook.Worksheets["Sheet1"];
            Cells cellsSrc = sheetSrc.Cells;
            Worksheet sheetDest = workbook.Worksheets[workbook.Worksheets.Add()];
            sheetDest.Name = "sheetDest";
            Cells cellsDest = sheetDest.Cells;
            cellsDest.CopyRows(cellsSrc, 0, 0, 43);

            checkCopyRows_Shape_001(workbook);
            workbook.Save(Constants.destPath + "testCopyRows.xls");
            workbook = new Workbook(Constants.destPath + "testCopyRows.xls");
            checkCopyRows_Shape_001(workbook);
            workbook.Save(Constants.destPath + "testCopyRows.xlsx");
            workbook = new Workbook(Constants.destPath + "testCopyRows.xlsx");
            checkCopyRows_Shape_001(workbook);
            workbook.Save(Constants.destPath + "testCopyRows.xml", SaveFormat.SpreadsheetML);
            workbook = new Workbook(Constants.destPath + "testCopyRows.xml");
            checkCopyRows_Shape_001(workbook);
            workbook.Save(Constants.destPath + "testCopyColumn.xls");
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyRows(Cells, int, int, int, CopyOptions) {#copyrows_1}

Copies data and formats of some whole rows.

```csharp
public void CopyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, 
    int rowNumber, CopyOptions copyOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells0 | Cells | Source Cells object contains data and formats to copy. |
| sourceRowIndex | Int32 | Source row index. |
| destinationRowIndex | Int32 | Destination row index. |
| rowNumber | Int32 | The copied row number. |
| copyOptions | CopyOptions | The copy options. |

### Examples

```csharp
// Called: destination.Cells.CopyRows(source.Cells, 0, 0, source.Cells.MaxDisplayRange.RowCount, options);
[Test]
        public void Method_CopyOptions_()
        {
            var book = new Workbook(Constants.sourcePath + "CellsNet44626.xlsx");
            var source = book.Worksheets[0];
            var destination = book.Worksheets[book.Worksheets.Add()];
            CopyOptions options = new CopyOptions();
            options.ReferToDestinationSheet = true;

            destination.Cells.CopyRows(source.Cells, 0, 0, source.Cells.MaxDisplayRange.RowCount, options);
            Assert.AreEqual(destination.Charts[0].NSeries[0].Values, "=Sheet2!$B$2:$B$4");
            Util.ReSave(book, SaveFormat.Xlsx);
            //book.Save(Constants.destPath + "CellsNet44626.xlsx");
        }
```

### See Also

* class [CopyOptions](../../copyoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyRows(Cells, int, int, int, CopyOptions, PasteOptions) {#copyrows_2}

Copies data and formats of some whole rows.

```csharp
public void CopyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, 
    int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells0 | Cells | Source Cells object contains data and formats to copy. |
| sourceRowIndex | Int32 | Source row index. |
| destinationRowIndex | Int32 | Destination row index. |
| rowNumber | Int32 | The copied row number. |
| copyOptions | CopyOptions | The copy options. |
| pasteOptions | PasteOptions | the options of pasting. |

### See Also

* class [CopyOptions](../../copyoptions/)
* class [PasteOptions](../../pasteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


