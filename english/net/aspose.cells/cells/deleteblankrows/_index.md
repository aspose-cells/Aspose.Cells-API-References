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
[Test]
        public void Method_DeleteBlankRows()
        {
            caseName = "testDeleteBlankRows_001";
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells[0, 0].PutValue(1);
            cells[2, 0].PutValue(true);

            Style style = common.GetStyle(workbook);
            StyleFlag sflag = new StyleFlag();
            sflag.Borders = true;
            cells.ApplyRowStyle(3, style, sflag);
            cells[6, 0].PutValue("abc");

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
// Called: workesheet.Cells.DeleteBlankRows(deleteOptions);
[Test]
        public void Method_DeleteOptions_()
        {
            string filePath = Constants.PivotTableSourcePath + @"NET47446_";

            Workbook workbook = new Workbook(filePath + "sample.xlsb");

            DeleteOptions deleteOptions = new DeleteOptions();
            deleteOptions.UpdateReference = true;

            foreach (Worksheet workesheet in workbook.Worksheets)
                workesheet.Cells.DeleteBlankRows(deleteOptions);

            workbook.Worksheets.RemoveAt("Play Check");
        }
```

### See Also

* class [DeleteOptions](../../deleteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


