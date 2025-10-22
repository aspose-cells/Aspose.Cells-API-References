##Range.ExportDataTable
Range method. Exports data in this range to a DataTable object
## ExportDataTable() {#exportdatatable}
Exports data in this range to a DataTable object.
```csharp
public DataTable ExportDataTable()
```
### Return Value
Exported DataTable object.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Data;
public class RangeMethodExportDataTableDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data in worksheet
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Price");
worksheet.Cells["A2"].PutValue("Laptop");
worksheet.Cells["B2"].PutValue(1200.50);
worksheet.Cells["A3"].PutValue("Phone");
worksheet.Cells["B3"].PutValue(899.99);
worksheet.Cells["A4"].PutValue("Tablet");
worksheet.Cells["B4"].PutValue(450.75);
// Create a range containing the data
Aspose.Cells.Range dataRange = worksheet.Cells.CreateRange("A1:B4");
try
{
// Export the range to DataTable
DataTable dataTable = dataRange.ExportDataTable();
Console.WriteLine("Data exported successfully to DataTable");
Console.WriteLine($"DataTable contains {dataTable.Rows.Count} rows and {dataTable.Columns.Count} columns");
// Display the exported data
foreach (DataRow row in dataTable.Rows)
{
Console.WriteLine($"{row[0]}: {row[1]}");
}
// Modify the DataTable and import back if needed
dataTable.Rows[0]["Price"] = 1300.00;
Console.WriteLine("\nModified first product price in DataTable to 1300.00");
}
catch (Exception ex)
{
Console.WriteLine($"Error exporting data: {ex.Message}");
}
// Save the workbook
workbook.Save("RangeMethodExportDataTableDemo.xlsx");
}
}
}
```
### See Also
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## ExportDataTable(ExportTableOptions) {#exportdatatable_1}
Exports data in this range to a DataTable object.
```csharp
public DataTable ExportDataTable(ExportTableOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| options | ExportTableOptions | The options of exporting range to datatable. |
### Return Value
Exported DataTable object.
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Data;
namespace AsposeCellsExamples
{
public class RangeMethodExportDataTableWithExportTableOptionsDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data in the worksheet
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue("Alice");
worksheet.Cells["B3"].PutValue(25);
// Name the range containing our data
Aspose.Cells.Range namedRange = worksheet.Cells.CreateRange("A1:B3");
namedRange.Name = "Names";
// Export the named range to DataTable with options
ExportTableOptions options = new ExportTableOptions();
options.ExportColumnName = true;
DataTable dataTable = namedRange.ExportDataTable(options);
// Display the results
Console.WriteLine("Exported DataTable:");
foreach (DataRow row in dataTable.Rows)
{
Console.WriteLine($"{row["Name"]}, {row["Age"]}");
}
}
}
}
```
### See Also
* class [ExportTableOptions](../../exporttableoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
