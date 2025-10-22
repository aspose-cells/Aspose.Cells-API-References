##SqlScriptColumnTypeMap.GetNumbericType
SqlScriptColumnTypeMap method. Gets numeric type in the database
## SqlScriptColumnTypeMap.GetNumbericType method
Gets numeric type in the database.
```csharp
public virtual string GetNumbericType()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;
namespace AsposeCellsExamples
{
public class SqlScriptColumnTypeMapMethodGetNumbericTypeDemo
{
public static void Run()
{
// Create an instance of SqlScriptColumnTypeMap
SqlScriptColumnTypeMap columnTypeMap = new SqlScriptColumnTypeMap();
// Get and display the numeric type mapping
string numericType = columnTypeMap.GetNumbericType();
Console.WriteLine("Numeric Type in Database: " + numericType);
// Create a simple workbook with numeric data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Number");
worksheet.Cells["A2"].PutValue(123.45);
// Save with SQL script options using the type mapping
SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
{
ColumnTypeMap = columnTypeMap
};
workbook.Save("NumericTypeDemo.sql", saveOptions);
}
}
}
```
### See Also
* class [SqlScriptColumnTypeMap](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)
