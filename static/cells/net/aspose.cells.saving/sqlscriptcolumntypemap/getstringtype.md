##SqlScriptColumnTypeMap.GetStringType
SqlScriptColumnTypeMap method. Gets string type in the database
## SqlScriptColumnTypeMap.GetStringType method
Gets string type in the database.
```csharp
public virtual string GetStringType()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;
namespace AsposeCellsExamples
{
public class SqlScriptColumnTypeMapMethodGetStringTypeDemo
{
public static void Run()
{
// Create an instance of SqlScriptColumnTypeMap
SqlScriptColumnTypeMap columnTypeMap = new SqlScriptColumnTypeMap();
// Get and display the default string type
string stringType = columnTypeMap.GetStringType();
Console.WriteLine("Default String Type: " + stringType);
// Create a simple workbook with string data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["A2"].PutValue("John Doe");
// Save with SQL script options using the type map
SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
{
ColumnTypeMap = columnTypeMap
};
workbook.Save("SqlScriptOutput.sql", saveOptions);
Console.WriteLine("SQL script saved with string type: " + stringType);
}
}
}
```
### See Also
* class [SqlScriptColumnTypeMap](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)
