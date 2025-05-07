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
// Called: cells.DeleteBlankColumns();
[Test]
        public void Method_DeleteBlankColumns()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSJAVA43010.xlsx");
            foreach (Worksheet worksheet in workbook.Worksheets)
            {

                Cells cells = worksheet.Cells;
                cells.DeleteBlankColumns();
            }
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
// Called: sheet.Cells.DeleteBlankColumns(options);
[Test]
        public void Method_DeleteOptions_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET45393.xls");
            DeleteBlankOptions options = new DeleteBlankOptions();
            options.UpdateReference = true;
            options.DrawingsAsBlank = false;

            foreach (Worksheet sheet in workbook.Worksheets)
            {
                sheet.Cells.DeleteBlankColumns(options);
                sheet.Cells.DeleteBlankRows(options);
            }
            Assert.AreEqual(1, workbook.Worksheets[0].Shapes.Count);
            Assert.IsTrue(workbook.Worksheets[0].Shapes[0].Width > 0);
            Assert.IsTrue(workbook.Worksheets[0].Shapes[0].Height > 0);
        }
```

### See Also

* class [DeleteOptions](../../deleteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


