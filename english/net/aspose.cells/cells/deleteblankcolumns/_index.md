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
[Test]
        public void Method_DeleteBlankColumns()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;TestDeleteBlankRows.xls&quot;);
            workbook.Worksheets[0].Cells.DeleteBlankRows();
            workbook.Worksheets[0].Cells.DeleteBlankColumns();
            Assert.AreEqual(workbook.Worksheets[0].Cells[&quot;C4&quot;].StringValue, &quot;sfsdf&quot;);
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
// Called: workbook.Worksheets[0].Cells.DeleteBlankColumns(deleteOptions);
[Test]
        public void Method_DeleteOptions_()
        {
            Workbook workbook  =new Workbook(Constants.sourcePath + &quot;CELLSNET-47741.xlsm&quot;);
            DeleteOptions deleteOptions = new DeleteOptions();
            deleteOptions.UpdateReference = true;

            workbook.Worksheets[0].Cells.DeleteBlankColumns(deleteOptions);
            workbook.Save(Constants.destPath + &quot;CELLSNET-47741.xlsm&quot;);
        }
```

### See Also

* class [DeleteOptions](../../deleteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


