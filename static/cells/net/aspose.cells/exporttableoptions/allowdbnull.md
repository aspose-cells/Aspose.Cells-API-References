##ExportTableOptions.AllowDBNull
ExportTableOptions property. This value indicates whether DBNulls are allowed in this table
## ExportTableOptions.AllowDBNull property
This value indicates whether DBNulls are allowed in this table.
```csharp
public bool AllowDBNull { get; set; }
```
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ExportTableOptionsPropertyAllowDBNullDemo
{
public static void Run()
{
// Create a sample workbook with test data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data with some empty cells
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue(""); // Empty cell
worksheet.Cells["B3"].PutValue(25);
// Export with AllowDBNull = true (default)
ExportTableOptions options1 = new ExportTableOptions
{
ExportColumnName = true,
AllowDBNull = true
};
DataTable table1 = worksheet.Cells.ExportDataTable(0, 0, 3, 2, options1);
Console.WriteLine("With AllowDBNull=true:");
Console.WriteLine("Row 2 Name: " + (table1.Rows[1]["Name"] == DBNull.Value ? "DBNull" : table1.Rows[1]["Name"]));
// Export with AllowDBNull = false
ExportTableOptions options2 = new ExportTableOptions
{
ExportColumnName = true,
AllowDBNull = false
};
DataTable table2 = worksheet.Cells.ExportDataTable(0, 0, 3, 2, options2);
Console.WriteLine("\nWith AllowDBNull=false:");
Console.WriteLine("Row 2 Name: " + (table2.Rows[1]["Name"] == DBNull.Value ? "DBNull" : table2.Rows[1]["Name"]));
}
}
}
```
### See Also
* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
