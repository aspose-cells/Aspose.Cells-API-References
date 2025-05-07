---
title: Cells.ImportDataGrid
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Imports a DataGrid into a worksheet
type: docs
url: /net/aspose.cells/cells/importdatagrid/
---
## ImportDataGrid(DataGrid, int, int, bool) {#importdatagrid}

Imports a DataGrid into a worksheet.

```csharp
public int ImportDataGrid(DataGrid dataGrid, int firstRow, int firstColumn, bool insertRows)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dataGrid | DataGrid | The DataGrid object to be imported. |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |
| insertRows | Boolean | Indicates whether extra rows are added to fit data. |

### Return Value

Total number of rows imported

### Examples

```csharp
// Called: sheet.Cells.ImportDataGrid(dataGrid, 1, 0, false);
[Test]
        public void Method_Boolean_()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            DataTable dataTable = new DataTable("Table1");

            dataTable.Columns.Add("Name", typeof(string));

            dataTable.Columns.Add("Date", typeof(DateTime));

            DataRow dr = dataTable.NewRow();

            dr[0] = "test";

            dr[1] = DateTime.Now;

            dataTable.Rows.Add(dr);

            System.Web.UI.WebControls.DataGrid dataGrid = new System.Web.UI.WebControls.DataGrid();

            dataGrid.DataSource = dataTable;

            dataGrid.UseAccessibleHeader = true;

            dataGrid.ShowHeader = true;

            dataGrid.DataBind();

            sheet.Cells.ImportDataGrid(dataGrid, 1, 0, false);

            sheet.AutoFitColumns();
            workbook.Save(Constants.destPath + "CellsNet44630.xlsx");
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportDataGrid(DataGrid, int, int, int, int, bool) {#importdatagrid_1}

Imports a DataGrid into a worksheet.

```csharp
public int ImportDataGrid(DataGrid dataGrid, int firstRow, int firstColumn, int totalRows, 
    int totalColumns, bool insertRows)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dataGrid | DataGrid | The DataGrid object to be imported. |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |
| totalRows | Int32 | Number of rows to be imported. |
| totalColumns | Int32 | Number of columns to be imported. |
| insertRows | Boolean | Indicates whether extra rows are added to fit data. |

### Return Value

Total number of rows imported

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportDataGrid(DataGrid, int, int, int, int, bool, bool) {#importdatagrid_2}

Imports a DataGrid into a worksheet.

```csharp
public int ImportDataGrid(DataGrid dataGrid, int firstRow, int firstColumn, int totalRows, 
    int totalColumns, bool insertRows, bool importStyle)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dataGrid | DataGrid | The DataGrid object to be imported. |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |
| totalRows | Int32 | Number of rows to be imported. |
| totalColumns | Int32 | Number of columns to be imported. |
| insertRows | Boolean | Indicates whether extra rows are added to fit data. |
| importStyle | Boolean | Indicates whether importing the cell style. |

### Return Value

Total number of rows imported

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


