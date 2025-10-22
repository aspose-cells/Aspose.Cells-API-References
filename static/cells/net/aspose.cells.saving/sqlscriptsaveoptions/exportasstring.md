##SqlScriptSaveOptions.ExportAsString
SqlScriptSaveOptions property. Indicates whether exporting all data as string value
## SqlScriptSaveOptions.ExportAsString property
Indicates whether exporting all data as string value.
```csharp
public bool ExportAsString { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;
namespace AsposeCellsExamples
{
public class SqlScriptSaveOptionsPropertyExportAsStringDemo
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
// Configure SQL export options
SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
{
TableName = "Employees",
ExportAsString = true, // Demonstrating ExportAsString property
HasHeaderRow = true
};
// Save with string export enabled
workbook.Save("ExportAsString_True.sql", saveOptions);
// Change to false and save again
saveOptions.ExportAsString = false;
workbook.Save("ExportAsString_False.sql", saveOptions);
Console.WriteLine("SQL scripts saved with different ExportAsString settings.");
}
}
}
```
### See Also
* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)
