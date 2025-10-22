##SqlScriptSaveOptions.TableName
SqlScriptSaveOptions property. Gets and sets the table name
## SqlScriptSaveOptions.TableName property
Gets and sets the table name.
```csharp
public string TableName { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;
namespace AsposeCellsExamples
{
public class SqlScriptSaveOptionsPropertyTableNameDemo
{
public static void Run()
{
// Create a sample workbook with some data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue("Alice");
worksheet.Cells["B3"].PutValue(25);
// Configure SQL save options with custom table name
SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions();
saveOptions.TableName = "Employees"; // Demonstrating TableName property
saveOptions.CreateTable = true;
saveOptions.OperatorType = SqlScriptOperatorType.Insert;
// Save as SQL script
workbook.Save("output.sql", saveOptions);
Console.WriteLine("SQL Script generated with table name 'Employees'");
}
}
}
```
### See Also
* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)
