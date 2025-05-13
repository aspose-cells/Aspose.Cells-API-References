---
title: Cells.ExportDataTableAsString
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Exports data in the Cells collection to a DataTable object
type: docs
url: /net/aspose.cells/cells/exportdatatableasstring/
---
## ExportDataTableAsString(int, int, int, int) {#exportdatatableasstring}

Exports data in the [`Cells`](../) collection to a DataTable object.

```csharp
public DataTable ExportDataTableAsString(int firstRow, int firstColumn, int totalRows, 
    int totalColumns)
```

| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | The row number of the first cell to export out. |
| firstColumn | Int32 | The column number of the first cell to export out. |
| totalRows | Int32 | Number of rows to be imported. |
| totalColumns | Int32 | Number of columns to be imported. |

### Return Value

Exported DataTable object.

### Remarks

All data in the [`Cells`](../) collection are converted to strings.

### Examples

```csharp
// Called: DataTable datatable = cells.ExportDataTableAsString(0, 0, 65536, 256);
private void Cells_Method_ExportDataTableAsString(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            DataTable datatable = cells.ExportDataTableAsString(0, 0, 65536, 256);
            testAreEqual(65536, datatable.Rows.Count, caseName);
            testAreEqual(256, datatable.Columns.Count, caseName);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ExportDataTableAsString(int, int, int, int, bool) {#exportdatatableasstring_1}

Exports data in the [`Cells`](../) collection to a DataTable object.

```csharp
public DataTable ExportDataTableAsString(int firstRow, int firstColumn, int totalRows, 
    int totalColumns, bool exportColumnName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | The row number of the first cell to export out. |
| firstColumn | Int32 | The column number of the first cell to export out. |
| totalRows | Int32 | Number of rows to be imported. |
| totalColumns | Int32 | Number of columns to be imported. |
| exportColumnName | Boolean | Indicates whether the data in the first row are exported to the column name of the DataTable. |

### Return Value

Exported DataTable object.

### Remarks

All data in the [`Cells`](../) collection are converted to strings.

### Examples

```csharp
// Called: dt = book.Worksheets[0].Cells.ExportDataTableAsString(0, 0, row, column, true);
public void Cells_Method_ExportDataTableAsString()
{
    Workbook book = new Workbook(Constants.sourcePath + "example.xls");
    DataTable dt = new DataTable();
    DataSet ds = new DataSet();
    int column = book.Worksheets[0].Cells.MaxDataColumn + 1;
    int row = book.Worksheets[0].Cells.MaxDataRow + 1;
    dt = book.Worksheets[0].Cells.ExportDataTableAsString(0, 0, row, column, true);
    ds.Tables.Add(dt);

}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


