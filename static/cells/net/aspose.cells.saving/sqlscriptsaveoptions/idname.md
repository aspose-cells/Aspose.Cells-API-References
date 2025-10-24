##SqlScriptSaveOptions.IdName
SqlScriptSaveOptions property. Gets and sets the name of id column
## SqlScriptSaveOptions.IdName property
Gets and sets the name of id column.
```csharp
public string IdName { get; set; }
```
### Remarks
If this property is set , a column will be inserted with automatical increment int value.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;
namespace AsposeCellsExamples
{
public class SqlScriptSaveOptionsPropertyIdNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("ID");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["A3"].PutValue(2);
worksheet.Cells["B1"].PutValue("Name");
worksheet.Cells["B2"].PutValue("Alice");
worksheet.Cells["B3"].PutValue("Bob");
// Configure SQL export options with IdName
SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
{
TableName = "Employees",
IdName = "ID",
CreateTable = true,
HasHeaderRow = true
};
// Save as SQL script
workbook.Save("Employees.sql", saveOptions);
Console.WriteLine("SQL script exported with IdName property");
}
}
}
```
### See Also
* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)
