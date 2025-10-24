##SqlScriptSaveOptions.ExportArea
SqlScriptSaveOptions property. Gets or sets the exporting range
## SqlScriptSaveOptions.ExportArea property
Gets or sets the exporting range.
```csharp
public CellArea ExportArea { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;
namespace AsposeCellsExamples
{
public class SqlScriptSaveOptionsPropertyExportAreaDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Fill worksheet with sample data
worksheet.Cells["A1"].PutValue("ID");
worksheet.Cells["B1"].PutValue("Name");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["B2"].PutValue("John");
worksheet.Cells["A3"].PutValue(2);
worksheet.Cells["B3"].PutValue("Jane");
// Configure SQL export options with ExportArea
SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
{
TableName = "Employees",
ExportArea = new CellArea { StartRow = 0, EndRow = 3, StartColumn = 0, EndColumn = 1 },
HasHeaderRow = true
};
// Save with specified export area (columns A1:B3)
workbook.Save("EmployeesExport.sql", saveOptions);
}
}
}
```
### See Also
* struct [CellArea](../../../aspose.cells/cellarea/)
* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)
