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
// Called: cells.ExportDataTableAsString(2, 2, 1048576, 16384);
[Test, ExpectedException(typeof(CellsException))]
#endif
        public void Method_Int32_()
        {
            caseName = "testExportDataTableAsString_Exception_009";
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            DataTable datatable = new DataTable();
            cells.ExportDataTableAsString(2, 2, 1048576, 16384);
            string msg = message + "cells.ExportDataTableAsString(2, 2, 1048576, 16384)";
            writeToExcel(caseName, msg);
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
// Called: System.Data.DataTable dt = excel.Worksheets[0].Cells.ExportDataTableAsString(0, 255, 5, 1, true);
[Test]
		public void Method_Boolean_()
		{
            Workbook excel = new Workbook(Constants.sourcePath + "exportlastcol.xls");
			System.Data.DataTable dt = excel.Worksheets[0].Cells.ExportDataTableAsString(0, 255, 5, 1, true);
			for(int i = 0; i < dt.Columns.Count; i ++)
				Console.WriteLine(dt.Columns[i].ColumnName);

			for(int i = 0; i < dt.Rows.Count; i ++)
			{
				System.Data.DataRow row = dt.Rows[i];
				for(int j = 0; j < row.ItemArray.Length; j ++)
				{
					Console.WriteLine(row[j].ToString());
				}
			}
		}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


