##SqlScriptSaveOptions.SqlScriptSaveOptions
SqlScriptSaveOptions constructor. Creates options for saving sql file
## SqlScriptSaveOptions constructor
Creates options for saving sql file.
```csharp
public SqlScriptSaveOptions()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;
namespace AsposeCellsExamples
{
public class SqlScriptSaveOptionsMethodCtorDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("ID");
worksheet.Cells["B1"].PutValue("Name");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["B2"].PutValue("John");
worksheet.Cells["A3"].PutValue(2);
worksheet.Cells["B3"].PutValue("Mary");
// Create SqlScriptSaveOptions using constructor
SqlScriptSaveOptions options = new SqlScriptSaveOptions();
options.OperatorType = SqlScriptOperatorType.Insert;
options.AddBlankLineBetweenRows = true;
// Save as SQL script
workbook.Save("output.sql", options);
// Output the generated SQL
Console.WriteLine("Generated SQL Script:");
Console.WriteLine(System.IO.File.ReadAllText("output.sql"));
}
}
}
```
### See Also
* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)
