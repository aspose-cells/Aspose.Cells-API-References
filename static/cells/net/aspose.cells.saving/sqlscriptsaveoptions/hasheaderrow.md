##SqlScriptSaveOptions.HasHeaderRow
SqlScriptSaveOptions property. Indicates whether the range contains header row
## SqlScriptSaveOptions.HasHeaderRow property
Indicates whether the range contains header row.
```csharp
public bool HasHeaderRow { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;
namespace AsposeCellsExamples
{
public class SqlScriptSaveOptionsPropertyHasHeaderRowDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add header row and sample data
worksheet.Cells["A1"].PutValue("ID");
worksheet.Cells["B1"].PutValue("Name");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["B2"].PutValue("Alice");
worksheet.Cells["A3"].PutValue(2);
worksheet.Cells["B3"].PutValue("Bob");
// Configure SQL export options with HasHeaderRow=true
SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
{
TableName = "Employees",
HasHeaderRow = true,
CreateTable = true
};
// Save as SQL script
workbook.Save("Employees.sql", saveOptions);
Console.WriteLine("SQL script with header row exported successfully.");
}
}
}
```
### See Also
* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)
