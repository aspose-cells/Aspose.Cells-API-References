##SqlScriptSaveOptions.OperatorType
SqlScriptSaveOptions property. Gets and sets the operator type of sql
## SqlScriptSaveOptions.OperatorType property
Gets and sets the operator type of sql.
```csharp
public SqlScriptOperatorType OperatorType { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Saving;
namespace AsposeCellsExamples
{
public class SqlScriptSaveOptionsPropertyOperatorTypeDemo
{
public static void Run()
{
// Create a sample workbook with test data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Id");
worksheet.Cells["B1"].PutValue("Name");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["B2"].PutValue("John");
worksheet.Cells["A3"].PutValue(2);
worksheet.Cells["B3"].PutValue("Jane");
// Configure SQL save options
SqlScriptSaveOptions options = new SqlScriptSaveOptions();
options.OperatorType = SqlScriptOperatorType.Delete;
options.IdName = "Id";
options.Separator = '\n';
options.AddBlankLineBetweenRows = true;
options.CreateTable = true;
// Save to memory stream and get SQL script as string
using (MemoryStream stream = new MemoryStream())
{
workbook.Save(stream, options);
stream.Position = 0;
using (StreamReader reader = new StreamReader(stream))
{
string sqlScript = reader.ReadToEnd();
// Output the generated SQL
Console.WriteLine("Generated SQL Script:");
Console.WriteLine(sqlScript);
}
}
}
}
}
```
### See Also
* enum [SqlScriptOperatorType](../../sqlscriptoperatortype/)
* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)
