---
title: Cells.Import
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Import data from data view
type: docs
url: /net/aspose.cells/cells/import/
---
## Cells.Import method

Import data from data view.

```csharp
[Obsolete("Use Cells.ImportData(IDataReader,int,int,ImportTableOptions) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Import(IDataReader dataReader, int firstRow, int firstColumn, ImportTableOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dataReader | IDataReader | The IDataReader object to be imported. |
| firstRow | Int32 | First row index. |
| firstColumn | Int32 | First column index. |
| options | ImportTableOptions | The import options |

### Return Value

Total number of rows imported.

### Remarks

NOTE: This member is now obsolete. Instead, please use Cells.ImportData(IDataReader,int,int,ImportTableOptions) method, instead. This property will be removed 12 months later since December 2018. Aspose apologizes for any inconvenience you may have experienced.

### See Also

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


