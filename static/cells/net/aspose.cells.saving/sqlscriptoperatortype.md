##Enum SqlScriptOperatorType
Aspose.Cells.Saving.SqlScriptOperatorType enum. Represents the type of operating data
## SqlScriptOperatorType enumeration
Represents the type of operating data.
```csharp
public enum SqlScriptOperatorType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Insert | `0` | Insert data. |
| Update | `1` | Update data. |
| Delete | `2` | Delete data. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Saving;
using System;
public class SqlScriptOperatorTypeDemo
{
public static void SqlScriptOperatorTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("ID");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["A3"].PutValue(2);
worksheet.Cells["A4"].PutValue(3);
worksheet.Cells["B1"].PutValue("Name");
worksheet.Cells["B2"].PutValue("Alice");
worksheet.Cells["B3"].PutValue("Bob");
worksheet.Cells["B4"].PutValue("Charlie");
// Create SqlScriptSaveOptions and set properties
SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
{
CheckIfTableExists = true,
AddBlankLineBetweenRows = true,
Separator = ';',
OperatorType = SqlScriptOperatorType.Insert,
PrimaryKey = 0,
CreateTable = true,
IdName = "ID",
StartId = 1,
TableName = "SampleTable",
ExportAsString = false,
ExportArea = new CellArea { StartRow = 1, StartColumn = 0, EndRow = 3, EndColumn = 1 },
HasHeaderRow = true
};
// Save the workbook as SQL script
workbook.Save("SqlScriptOperatorTypeExample.sql", saveOptions);
// Output the results
Console.WriteLine("SQL script has been saved successfully.");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)
