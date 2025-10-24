##SqlScriptSaveOptions.ColumnTypeMap
SqlScriptSaveOptions property. Gets and sets the map of column type for different database
## SqlScriptSaveOptions.ColumnTypeMap property
Gets and sets the map of column type for different database.
```csharp
public SqlScriptColumnTypeMap ColumnTypeMap { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;
namespace AsposeCellsExamples
{
public class SqlScriptSaveOptionsPropertyColumnTypeMapDemo
{
public static void Run()
{
// Create a custom column type map
SqlScriptColumnTypeMap customTypeMap = new SqlScriptColumnTypeMap();
// Create SQL save options
SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
{
TableName = "Employees",
CreateTable = true,
ColumnTypeMap = customTypeMap,
CheckIfTableExists = true,
ExportAsString = false
};
// Create sample workbook with data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add headers
worksheet.Cells["A1"].PutValue("ID");
worksheet.Cells["B1"].PutValue("Name");
worksheet.Cells["C1"].PutValue("Salary");
// Add data rows
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["B2"].PutValue("John Smith");
worksheet.Cells["C2"].PutValue(5000.50);
worksheet.Cells["A3"].PutValue(2);
worksheet.Cells["B3"].PutValue("Jane Doe");
worksheet.Cells["C3"].PutValue(6500.75);
// Save as SQL script
workbook.Save("EmployeeData.sql", saveOptions);
Console.WriteLine("SQL script generated successfully with custom column type mapping.");
}
}
}
```
### See Also
* class [SqlScriptColumnTypeMap](../../sqlscriptcolumntypemap/)
* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)
