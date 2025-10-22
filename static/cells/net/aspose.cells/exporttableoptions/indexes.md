##ExportTableOptions.Indexes
ExportTableOptions property. The indexes of columns/rows which should be exported out
## ExportTableOptions.Indexes property
The indexes of columns/rows which should be exported out.
```csharp
public int[] Indexes { get; set; }
```
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ExportTableOptionsPropertyIndexesDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["C1"].PutValue("Department");
worksheet.Cells["D1"].PutValue("Salary");
worksheet.Cells["E1"].PutValue("Join Date");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["C2"].PutValue("IT");
worksheet.Cells["D2"].PutValue(5000);
worksheet.Cells["E2"].PutValue("2020-01-15");
worksheet.Cells["A3"].PutValue("Alice");
worksheet.Cells["B3"].PutValue(28);
worksheet.Cells["C3"].PutValue("HR");
worksheet.Cells["D3"].PutValue(4500);
worksheet.Cells["E3"].PutValue("2019-11-20");
// Create export options and specify column indexes to export (in reverse order)
ExportTableOptions options = new ExportTableOptions();
options.ExportColumnName = true;
options.Indexes = new int[] { 4, 2, 0 }; // Export columns: Join Date, Department, Name
// Export data with specified column indexes
DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 3, 5, options);
// Display the exported data
foreach (DataRow row in dataTable.Rows)
{
Console.WriteLine($"{row[0]}, {row[1]}, {row[2]}");
}
}
}
}
```
### See Also
* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
