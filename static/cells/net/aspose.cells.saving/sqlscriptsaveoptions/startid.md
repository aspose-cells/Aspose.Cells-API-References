##SqlScriptSaveOptions.StartId
SqlScriptSaveOptions property. Gets and sets the start id
## SqlScriptSaveOptions.StartId property
Gets and sets the start id.
```csharp
public int StartId { get; set; }
```
### Remarks
Only works when [`IdName`](../idname/) is set.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;
namespace AsposeCellsExamples
{
public class SqlScriptSaveOptionsPropertyStartIdDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("ID");
worksheet.Cells["B1"].PutValue("Name");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["B2"].PutValue("John");
worksheet.Cells["A3"].PutValue(2);
worksheet.Cells["B3"].PutValue("Jane");
// Configure SQL export options with StartId set to 100
SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
{
TableName = "Employees",
IdName = "ID",
StartId = 100, // Demonstrating StartId property
HasHeaderRow = true,
OperatorType = SqlScriptOperatorType.Insert
};
// Save as SQL script
workbook.Save("Employees_WithStartId.sql", saveOptions);
}
}
}
```
### See Also
* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)
