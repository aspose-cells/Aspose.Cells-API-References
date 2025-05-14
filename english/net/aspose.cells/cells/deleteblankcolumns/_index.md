---
title: Cells.DeleteBlankColumns
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Delete all blank columns which do not contain any data
type: docs
url: /net/aspose.cells/cells/deleteblankcolumns/
---
## DeleteBlankColumns() {#deleteblankcolumns}

Delete all blank columns which do not contain any data.

```csharp
public void DeleteBlankColumns()
```

### Examples

```csharp
// Called: workbook.Worksheets[0].Cells.DeleteBlankColumns();
public void Cells_Method_DeleteBlankColumns()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "TestDeleteBlankRows.xls");
    workbook.Worksheets[0].Cells.DeleteBlankRows();
    workbook.Worksheets[0].Cells.DeleteBlankColumns();
    Assert.AreEqual(workbook.Worksheets[0].Cells["C4"].StringValue, "sfsdf");
    workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteBlankColumns(DeleteOptions) {#deleteblankcolumns_1}

Delete all blank columns which do not contain any data.

```csharp
public void DeleteBlankColumns(DeleteOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| options | DeleteOptions | The options of deleting range. |

### Examples

```csharp
// Called: cells.DeleteBlankColumns(options);
public void Cells_Method_DeleteBlankColumns()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    Worksheet sheet = wb.Worksheets[0];

    DeleteOptions options = new DeleteOptions();
    options.UpdateReference = true;
    Cells cells = sheet.Cells;
    cells.DeleteBlankColumns(options);
    cells.DeleteBlankRows(options);
    Assert.AreEqual(63, cells.MaxDataRow);
    Assert.AreEqual(67, wb.Worksheets[0].Shapes[1].UpperLeftRow); //old value is 80, changed for CELLSNET-57838
    Util.SetHintMessage(cells[0, 2], "File should not be corrupted when openning by ms excel 2010 or higher");
    Util.SaveManCheck(wb, "", "example.xlsx");
    Util.SaveManCheck(wb, "", "example.xls");
}
```

### See Also

* class [DeleteOptions](../../deleteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


