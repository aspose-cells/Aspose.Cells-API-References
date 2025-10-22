##SqlScriptSaveOptions.PrimaryKey
SqlScriptSaveOptions property. Represents which column is primary key of the data table
## SqlScriptSaveOptions.PrimaryKey property
Represents which column is primary key of the data table.
```csharp
public int PrimaryKey { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;
namespace AsposeCellsExamples
{
public class SqlScriptSaveOptionsPropertyPrimaryKeyDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("ID");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["A3"].PutValue(2);
worksheet.Cells["B1"].PutValue("Name");
worksheet.Cells["B2"].PutValue("Alice");
worksheet.Cells["B3"].PutValue("Bob");
// Configure SQL export options with PrimaryKey set to first column (0)
SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
{
PrimaryKey = 0,
TableName = "Employees",
CreateTable = true,
HasHeaderRow = true
};
// Save as SQL script
workbook.Save("EmployeesExport.sql", saveOptions);
Console.WriteLine("SQL script exported with PrimaryKey set to column 0 (ID)");
}
}
}
```
### See Also
* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)
