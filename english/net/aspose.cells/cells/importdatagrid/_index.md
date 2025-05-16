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
public void Cells_Method_ImportDataGrid()
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
    workbook.Save(Constants.destPath + "example.xlsx");
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

### Examples

```csharp
namespace AsposeCellsExamples.CellsMethodImportDataGridWithDataGridInt32Int32Int32Int32BoDemo
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class CellsMethodImportDataGridWithDataGridInt32Int32Int32Int32BoDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create and populate DataTable
            DataTable dt = new DataTable("Employees");
            dt.Columns.Add("Name", typeof(string));
            dt.Columns.Add("Department", typeof(string));
            dt.Rows.Add("John Smith", "Engineering");
            dt.Rows.Add("Emily Johnson", "Marketing");
            dt.Rows.Add("Michael Brown", "Sales");

            try
            {
                // Import DataTable starting at cell B3 (third row, second column)
                var options = new ImportTableOptions();
                worksheet.Cells.ImportData(dt, 2, 1, options);

                Console.WriteLine($"Imported {dt.Rows.Count} rows and {dt.Columns.Count} columns successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during import: {ex.Message}");
            }

            workbook.Save("CellsMethodImportDataGridDemo.xlsx");
        }
    }
}
```

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

### Examples

```csharp
namespace AsposeCellsExamples.CellsMethodImportDataGridWithDataGridInt32Int32Int32Int32BoDemo1
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class CellsMethodImportDataGridWithDataGridInt32Int32Int32Int32BoDemo1
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create a DataTable and populate with sample data
            DataTable dataTable = new DataTable();
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Age", typeof(int));
            dataTable.Rows.Add("John Doe", 30);
            dataTable.Rows.Add("Jane Smith", 25);

            try
            {
                // Configure import options
                ImportTableOptions importOptions = new ImportTableOptions();
                importOptions.IsFieldNameShown = true; // Preserve column headers
                importOptions.ConvertNumericData = true; // Corrected property name

                // Import data from DataTable into the worksheet
                int importedRows = worksheet.Cells.ImportData(dataTable, 0, 0, importOptions);

                Console.WriteLine($"Imported {importedRows} rows into the spreadsheet.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportData: {ex.Message}");
            }

            // Save the modified workbook
            workbook.Save("ImportDataGridWithDataGridDemo.xlsx");
        }
    }
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


