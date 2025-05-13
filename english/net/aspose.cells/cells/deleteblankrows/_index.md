---
title: Cells.DeleteBlankRows
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Delete all blank rows which do not contain any data or other object
type: docs
url: /net/aspose.cells/cells/deleteblankrows/
---
## DeleteBlankRows() {#deleteblankrows}

Delete all blank rows which do not contain any data or other object.

```csharp
public void DeleteBlankRows()
```

### Examples

```csharp
// Called: cells.DeleteBlankRows();
public void Cells_Method_DeleteBlankRows()
{
    caseName = "testDeleteBlankRows_002";
    Workbook workbook = new Workbook();            
    workbook = new Workbook(Constants.sourcePath + "example.xls");
    Cells cells = workbook.Worksheets[0].Cells;
    cells.DeleteBlankRows();

    checkDeleteBlankRows_001(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
    checkDeleteBlankRows_001(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
    checkDeleteBlankRows_001(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.SpreadsheetML);
    checkDeleteBlankRows_001(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteBlankRows(DeleteOptions) {#deleteblankrows_1}

Delete all blank rows which do not contain any data or some special objects such as visible comment, pivot table.

```csharp
public void DeleteBlankRows(DeleteOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| options | DeleteOptions | The options of deleting range. |

### Remarks

For blank rows that will be deleted, it is not only required that [`IsBlank`](../../row/isblank/) should be true, but also there should be no visible comment defined for any cell in those rows, and no pivot table whose range intersects with them.

### Examples

```csharp
// Called: sheet.Cells.DeleteBlankRows(options);
public void Cells_Method_DeleteBlankRows()
{
    var workbook = new Workbook(Constants.sourcePath + "example.xls");
    DeleteOptions options = new DeleteOptions();
    options.UpdateReference = true;

    foreach (Worksheet sheet in workbook.Worksheets)
    {
        sheet.Cells.DeleteBlankColumns(options);
        sheet.Cells.DeleteBlankRows(options);
    }
    Assert.AreEqual(0, workbook.Worksheets[0].Cells.GetColumnWidthPixel(12));
    Assert.AreEqual(0, workbook.Worksheets[0].Cells.GetRowHeight(30));
    workbook.Save(Constants.destPath + "example.xls");
}
```

### See Also

* class [DeleteOptions](../../deleteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


