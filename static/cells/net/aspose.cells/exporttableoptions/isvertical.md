##ExportTableOptions.IsVertical
ExportTableOptions property. True if a row in Workbook file represents a row in DataTable. False if a column in Workbook file represents a row in DataTable
## ExportTableOptions.IsVertical property
True if a row in Workbook file represents a row in DataTable. False if a column in Workbook file represents a row in DataTable.
```csharp
public bool IsVertical { get; set; }
```
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ExportTableOptionsPropertyIsVerticalDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Create sample data in worksheet
cells["A1"].PutValue("Name");
cells["B1"].PutValue("Age");
cells["A2"].PutValue("John");
cells["B2"].PutValue(25);
cells["A3"].PutValue("Alice");
cells["B3"].PutValue(30);
// Create DataTable
DataTable dt = new DataTable();
dt.Columns.Add("Column1", typeof(string));
dt.Columns.Add("Column2", typeof(int));
// Set ExportTableOptions with IsVertical = true
ExportTableOptions options = new ExportTableOptions();
options.IsVertical = true;
options.ExportColumnName = true;
options.DataTable = dt;
// Export data vertically
cells.ExportDataTable(0, 0, 2, 2, options);
// Display the exported DataTable
foreach (DataRow row in dt.Rows)
{
Console.WriteLine($"{row[0]}, {row[1]}");
}
}
}
}
```
### See Also
* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
