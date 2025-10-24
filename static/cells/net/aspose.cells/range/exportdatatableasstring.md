##Range.ExportDataTableAsString
Range method. Exports data in this range to a DataTable object
## Range.ExportDataTableAsString method
Exports data in this range to a DataTable object.
```csharp
public DataTable ExportDataTableAsString()
```
### Return Value
Exported DataTable object.
### Remarks
All data in the [`Cells`](../../cells/) collection are converted to strings.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Data;
public class RangeMethodExportDataTableAsStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(25);
worksheet.Cells["A3"].PutValue("Alice");
worksheet.Cells["B3"].PutValue(30);
// Get the range containing data
Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");
try
{
// Call the ExportDataTableAsString method
DataTable dataTable = range.ExportDataTableAsString();
// Display the exported data
Console.WriteLine("Exported DataTable:");
foreach (DataRow row in dataTable.Rows)
{
Console.WriteLine($"{row[0]}, {row[1]}");
}
// Save the workbook
workbook.Save("RangeMethodExportDataTableAsStringDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing ExportDataTableAsString method: {ex.Message}");
}
}
}
}
```
### See Also
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
