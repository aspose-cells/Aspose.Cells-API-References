##SqlScriptSaveOptions.CheckIfTableExists
SqlScriptSaveOptions property. Check if the table name exists before creating
## SqlScriptSaveOptions.CheckIfTableExists property
Check if the table name exists before creating
```csharp
public bool CheckIfTableExists { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;
namespace AsposeCellsExamples
{
public class SqlScriptSaveOptionsPropertyCheckIfTableExistsDemo
{
public static void Run()
{
// Create a sample workbook with test data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("ID");
worksheet.Cells["B1"].PutValue("Name");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["B2"].PutValue("John");
worksheet.Cells["A3"].PutValue(2);
worksheet.Cells["B3"].PutValue("Jane");
// Configure SQL save options
SqlScriptSaveOptions sqlOptions = new SqlScriptSaveOptions();
sqlOptions.CreateTable = true;
sqlOptions.CheckIfTableExists = true;
sqlOptions.OperatorType = SqlScriptOperatorType.Insert;
// Save to SQL script file
workbook.Save("output.sql", sqlOptions);
// Read and output the generated SQL
string sqlScript = System.IO.File.ReadAllText("output.sql");
Console.WriteLine("Generated SQL Script:");
Console.WriteLine(sqlScript);
}
}
}
```
### See Also
* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)
