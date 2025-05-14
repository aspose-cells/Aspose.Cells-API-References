---
title: Cells.DeleteColumns
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Deletes several columns
type: docs
url: /net/aspose.cells/cells/deletecolumns/
---
## DeleteColumns(int, int, bool) {#deletecolumns_1}

Deletes several columns.

```csharp
public void DeleteColumns(int columnIndex, int totalColumns, bool updateReference)
```

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Index of the first column to be deleted. |
| totalColumns | Int32 | Count of columns to be deleted. |
| updateReference | Boolean | Indicates whether update references in other worksheets. |

### Examples

```csharp
// Called: ws.Cells.DeleteColumns(0, 1, true); // <-- This causes #REF too
public void Cells_Method_DeleteColumns()
{
    var file = Constants.sourcePath + @"example.xlsx";
    var wb = new Workbook(file);
    var ws = wb.Worksheets[0];
    // ws.Cells.InsertColumns(0, 4, true); // <-- This causes #REF 
    //ws.Cells.InsertColumns(0, 4); // <-- This causes #REF too
    ws.Cells.DeleteColumns(0, 1, true); // <-- This causes #REF too
    Assert.AreEqual("=SUBTOTAL(109,[Amount])",ws.Cells["C6"].Formula);

    wb = new Workbook(file);
    ws = wb.Worksheets[0];
    ws.Cells.InsertColumns(0, 4, true); // <-- This causes #REF 
    //ws.Cells.InsertColumns(0, 4); // <-- This causes #REF too
   // ws.Cells.DeleteColumns(0, 1, true); // <-- This causes #REF too
    Assert.AreEqual("=SUBTOTAL(109,[Amount])", ws.Cells["H6"].Formula);
    //wb.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteColumns(int, int, DeleteOptions) {#deletecolumns}

Deletes several columns.

```csharp
public void DeleteColumns(int columnIndex, int totalColumns, DeleteOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Index of the first column to be deleted. |
| totalColumns | Int32 | Count of columns to be deleted. |
| options | DeleteOptions | Options for the deleting operation |

### See Also

* class [DeleteOptions](../../deleteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


