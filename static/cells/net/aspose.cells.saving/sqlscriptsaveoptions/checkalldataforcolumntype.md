##SqlScriptSaveOptions.CheckAllDataForColumnType
SqlScriptSaveOptions property. Check all data to find columns data type
## SqlScriptSaveOptions.CheckAllDataForColumnType property
Check all data to find columns' data type.
```csharp
public bool CheckAllDataForColumnType { get; set; }
```
### Remarks
The default value is false, we only check the first row for performance. If this property is true and the columns contains mixed value type, the columns' type will be text.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;
namespace AsposeCellsExamples
{
public class SqlScriptSaveOptionsPropertyCheckAllDataForColumnTypeDemo
{
public static void Run()
{
// Create a sample workbook with test data
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
// Add sample data with mixed types
sheet.Cells["A1"].PutValue("First_name");
sheet.Cells["B1"].PutValue("Last_name");
sheet.Cells["C1"].PutValue("age");
sheet.Cells["D1"].PutValue("tax");
sheet.Cells["A2"].PutValue("John");
sheet.Cells["B2"].PutValue("Doe");
sheet.Cells["C2"].PutValue(30);
sheet.Cells["D2"].PutValue("10%");
sheet.Cells["A3"].PutValue("Jane");
sheet.Cells["B3"].PutValue("Smith");
sheet.Cells["C3"].PutValue(25);
sheet.Cells["D3"].PutValue(0.15);
// Configure SQL save options
SqlScriptSaveOptions sqlSaveOptions = new SqlScriptSaveOptions();
sqlSaveOptions.OperatorType = SqlScriptOperatorType.Insert;
sqlSaveOptions.CreateTable = true;
sqlSaveOptions.CheckAllDataForColumnType = true; // This will examine all data to determine column types
// Save as SQL script - Save method doesn't return string, so we need to save first then read the file
wb.Save("output.sql", sqlSaveOptions);
// Read the generated SQL script
string sqlScript = System.IO.File.ReadAllText("output.sql");
Console.WriteLine("SQL Script generated:");
Console.WriteLine(sqlScript);
}
}
}
```
### See Also
* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)
