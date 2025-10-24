##SqlScriptSaveOptions.CreateTable
SqlScriptSaveOptions property. Indicates whether exporting sql of creating table
## SqlScriptSaveOptions.CreateTable property
Indicates whether exporting sql of creating table.
```csharp
public bool CreateTable { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;
namespace AsposeCellsExamples
{
public class SqlScriptSaveOptionsPropertyCreateTableDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("ID");
worksheet.Cells["B1"].PutValue("Name");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["B2"].PutValue("John");
worksheet.Cells["A3"].PutValue(2);
worksheet.Cells["B3"].PutValue("Jane");
// Configure SQL export options with CreateTable enabled
SqlScriptSaveOptions options = new SqlScriptSaveOptions
{
CreateTable = true,
TableName = "Employees",
HasHeaderRow = true
};
// Save as SQL script
workbook.Save("output.sql", options);
}
}
}
```
### See Also
* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)
