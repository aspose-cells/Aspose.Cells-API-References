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

### See Also

* class [DeleteOptions](../../deleteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


