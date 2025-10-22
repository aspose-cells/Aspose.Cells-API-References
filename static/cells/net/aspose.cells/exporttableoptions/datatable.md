##ExportTableOptions.DataTable
ExportTableOptions property. Gets and sets the DataTable which columns data type is assigned
## ExportTableOptions.DataTable property
Gets and sets the DataTable which columns' data type is assigned.
```csharp
public DataTable DataTable { get; set; }
```
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ExportTableOptionsPropertyDataTableDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Add sample data to cells
cells["A1"].PutValue("Column1");
cells["B1"].PutValue("Column2");
cells["A2"].PutValue(100);
cells["B2"].PutValue("Text1");
cells["A3"].PutValue(200);
cells["B3"].PutValue("Text2");
// Create DataTable and define columns
DataTable dt = new DataTable();
dt.Columns.Add("NumericData", typeof(double));
dt.Columns.Add("TextData", typeof(string));
// Configure export options
ExportTableOptions options = new ExportTableOptions();
options.ExportColumnName = true;
options.Indexes = new int[] { 0, 1 }; // Export both columns
options.DataTable = dt;
// Export data to DataTable
cells.ExportDataTable(0, 0, 3, 2, options);
// Display exported data
Console.WriteLine("Exported DataTable:");
foreach (DataRow row in dt.Rows)
{
Console.WriteLine($"{row["NumericData"]}, {row["TextData"]}");
}
}
}
}
```
### See Also
* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
