##Cells.ImportData
Cells method. Import data from custom data table
## ImportData(ICellsDataTable, int, int, ImportTableOptions) {#importdata}
Import data from custom data table.
```csharp
public int ImportData(ICellsDataTable table, int firstRow, int firstColumn,
ImportTableOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| table | ICellsDataTable | The custom data table. |
| firstRow | Int32 | First row index. |
| firstColumn | Int32 | First column index. |
| options | ImportTableOptions | The import options |
### Examples
```csharp
using System;
using System.Collections;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodImportDataWithICellsDataTableInt32Int32ImporDemo
{
public static void Run()
{
Workbook wb = new Workbook();
ArrayList dataLists = new ArrayList();
dataLists.Add(new object[] { "Name", "Age", "Gender" });
dataLists.Add(new object[] { "Alice", 30, "Female" });
dataLists.Add(new object[] { "Bob", 25, "Male" });
dataLists.Add(new object[] { "Charlie", 35, "Male" });
ICellsDataTable dt = wb.CellsDataTableFactory.GetInstance(dataLists, true);
wb.Worksheets[0].Cells.ImportData(dt, 0, 0, new ImportTableOptions());
Console.WriteLine("Data imported to first worksheet:");
Console.WriteLine(wb.Worksheets[0].Cells["A2"].StringValue);
wb.Save("output.xlsx");
}
}
}
```
### See Also
* interface [ICellsDataTable](../../icellsdatatable/)
* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## ImportData(DataTable, int, int, ImportTableOptions) {#importdata_1}
Import data from custom data table.
```csharp
public int ImportData(DataTable table, int firstRow, int firstColumn, ImportTableOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| table | DataTable | The DataTable object to be imported. |
| firstRow | Int32 | First row index. |
| firstColumn | Int32 | First column index. |
| options | ImportTableOptions | The import options |
### Return Value
Total number of rows imported.
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodImportDataWithDataTableInt32Int32ImportTableDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
// Create sample DataTable
DataTable dataTable = new DataTable("Products");
dataTable.Columns.Add("Product_ID", typeof(int));
dataTable.Columns.Add("Product_Name", typeof(string));
dataTable.Columns.Add("Units_In_Stock", typeof(int));
// Add sample data
DataRow row = dataTable.NewRow();
row[0] = 1;
row[1] = "Aniseed Syrup";
row[2] = 15;
dataTable.Rows.Add(row);
row = dataTable.NewRow();
row[0] = 2;
row[1] = "Boston Crab Meat";
row[2] = 123;
dataTable.Rows.Add(row);
// Set import options
ImportTableOptions importOptions = new ImportTableOptions();
importOptions.IsFieldNameShown = true;
// Import data starting at row 5, column 5
cells.ImportData(dataTable, 5, 5, importOptions);
// Save the workbook
workbook.Save("ImportDataDemo.xlsx");
}
}
}
```
### See Also
* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## ImportData(DataView, int, int, ImportTableOptions) {#importdata_2}
Import data from data view.
```csharp
public int ImportData(DataView dataView, int firstRow, int firstColumn, ImportTableOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| dataView | DataView | The DataView object to be imported. |
| firstRow | Int32 | First row index. |
| firstColumn | Int32 | First column index. |
| options | ImportTableOptions | The import options |
### Return Value
Total number of rows imported.
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodImportDataWithDataViewInt32Int32ImportTableODemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
// Create sample data table
DataTable dataTable = new DataTable("TestTable");
dataTable.Columns.Add("Column1", typeof(string));
dataTable.Columns.Add("Column2", typeof(int));
// Add sample data
dataTable.Rows.Add("Data1", 100);
dataTable.Rows.Add("Data2", 200);
dataTable.Rows.Add("Data3", 300);
// Create ImportTableOptions
ImportTableOptions options = new ImportTableOptions();
options.IsFieldNameShown = true;
options.InsertRows = true;
// Import data from DataView to cells starting at row 0, column 0
cells.ImportData(dataTable.DefaultView, 0, 0, options);
// Save the workbook
workbook.Save("ImportDataOutput.xlsx");
}
}
}
```
### See Also
* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## ImportData(IDataReader, int, int) {#importdata_3}
Imports data from a IDataReader object.
```csharp
public int ImportData(IDataReader reader, int firstRow, int firstColumn)
```
| Parameter | Type | Description |
| --- | --- | --- |
| reader | IDataReader | The IDataReader object which contains data. |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |
### Return Value
Total number of rows imported.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Data;
public class CellsMethodImportDataWithIDataReaderInt32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data table
DataTable dataTable = new DataTable("Employees");
dataTable.Columns.Add("ID", typeof(int));
dataTable.Columns.Add("Name", typeof(string));
dataTable.Columns.Add("Department", typeof(string));
dataTable.Rows.Add(1, "John Doe", "Engineering");
dataTable.Rows.Add(2, "Jane Smith", "Marketing");
dataTable.Rows.Add(3, "Mike Johnson", "Sales");
try
{
// Create IDataReader from DataTable
using (IDataReader dataReader = dataTable.CreateDataReader())
{
// Call ImportData method starting at cell A1 (row 0, column 0)
int importedRows = worksheet.Cells.ImportData(dataReader, 0, 0);
Console.WriteLine($"Imported {importedRows} rows successfully.");
Console.WriteLine($"Data starts at: A1 (Row 0, Column 0)");
}
// Auto-fit columns for better visibility
worksheet.AutoFitColumns();
}
catch (Exception ex)
{
Console.WriteLine($"Error executing ImportData method: {ex.Message}");
}
// Save the result
workbook.Save("ImportDataWithIDataReader.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## ImportData(IDataReader, int, int, ImportTableOptions) {#importdata_4}
Imports data from a IDataReader object.
```csharp
public int ImportData(IDataReader reader, int firstRow, int firstColumn, ImportTableOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| reader | IDataReader | The IDataReader object which contains data. |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |
| options | ImportTableOptions | The options of importing table. |
### Return Value
Total number of rows imported.
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodImportDataWithIDataReaderInt32Int32ImportTabDemo
{
public static void Run()
{
// Create a sample DataTable
DataTable dt = new DataTable("TestData");
dt.Columns.Add("Column1", typeof(string));
dt.Columns.Add("Column2", typeof(int));
dt.Columns.Add("Column3", typeof(DateTime));
// Add sample data
dt.Rows.Add("Data1", 100, DateTime.Now);
dt.Rows.Add("Data2", 200, DateTime.Now.AddDays(1));
dt.Rows.Add("Data3", 300, DateTime.Now.AddDays(2));
// Create DataTableReader
DataTableReader reader = dt.CreateDataReader();
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set import options
ImportTableOptions options = new ImportTableOptions();
options.IsFieldNameShown = true;
options.InsertRows = true;
options.ConvertNumericData = true;
options.DateFormat = "MM/dd/yyyy";
// Import data starting at row 5, column 0
int rowsImported = worksheet.Cells.ImportData(reader, 5, 0, options);
// Save the workbook
workbook.Save("ImportDataOutput.xlsx");
}
}
}
```
### See Also
* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
