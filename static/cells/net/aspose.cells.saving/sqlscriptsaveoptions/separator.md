##SqlScriptSaveOptions.Separator
SqlScriptSaveOptions property. Gets and sets character separator of sql script
## SqlScriptSaveOptions.Separator property
Gets and sets character separator of sql script.
```csharp
public char Separator { get; set; }
```
### Remarks
Only can be ' ' or '\n'. If the
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;
namespace AsposeCellsExamples
{
public class SqlScriptSaveOptionsPropertySeparatorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("ID");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["B1"].PutValue("Name");
worksheet.Cells["B2"].PutValue("John");
// Configure SQL save options with custom separator
SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
{
Separator = ';',
TableName = "Employees",
CreateTable = true,
HasHeaderRow = true
};
// Save with custom separator
workbook.Save("SqlScriptWithSeparator.sql", saveOptions);
Console.WriteLine("SQL script saved with custom separator.");
}
}
}
```
### See Also
* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)
