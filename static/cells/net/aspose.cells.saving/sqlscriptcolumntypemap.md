##Class SqlScriptColumnTypeMap
Aspose.Cells.Saving.SqlScriptColumnTypeMap class. Represents column type map
## SqlScriptColumnTypeMap class
Represents column type map.
```csharp
public class SqlScriptColumnTypeMap
```
## Constructors
| Name | Description |
| --- | --- |
| [SqlScriptColumnTypeMap](sqlscriptcolumntypemap/)() | The default constructor. |
## Methods
| Name | Description |
| --- | --- |
| virtual [GetNumbericType](../../aspose.cells.saving/sqlscriptcolumntypemap/getnumberictype/)() | Gets numeric type in the database. |
| virtual [GetStringType](../../aspose.cells.saving/sqlscriptcolumntypemap/getstringtype/)() | Gets string type in the database. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Saving;
using System;
public class SqlScriptColumnTypeMapDemo
{
public static void SqlScriptColumnTypeMapExample()
{
// Create an instance of SqlScriptColumnTypeMap
SqlScriptColumnTypeMap columnTypeMap = new SqlScriptColumnTypeMap();
// Demonstrate the usage of GetStringType and GetNumbericType methods
string stringType = columnTypeMap.GetStringType();
string numericType = columnTypeMap.GetNumbericType();
// Output the results to the console
Console.WriteLine("String Type in Database: " + stringType);
Console.WriteLine("Numeric Type in Database: " + numericType);
// Create an instance of SqlScriptSaveOptions and set the ColumnTypeMap
SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
{
ColumnTypeMap = columnTypeMap
};
// Create a workbook and add some data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("ID");
worksheet.Cells["B1"].PutValue("Name");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["B2"].PutValue("John Doe");
// Save the workbook as SQL script using the save options
workbook.Save("SqlScriptExample.sql", saveOptions);
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)
