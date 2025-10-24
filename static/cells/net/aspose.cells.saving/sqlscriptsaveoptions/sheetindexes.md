##SqlScriptSaveOptions.SheetIndexes
SqlScriptSaveOptions property. Represents the indexes of exported sheets
## SqlScriptSaveOptions.SheetIndexes property
Represents the indexes of exported sheets.
```csharp
public int[] SheetIndexes { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Saving;
using System;
public class SqlScriptSaveOptionsPropertySheetIndexesDemo
{
public static void Run()
{
// Create a new workbook with multiple sheets
Workbook workbook = new Workbook();
workbook.Worksheets.Add("Sheet2");
workbook.Worksheets.Add("Sheet3");
// Populate some data in all sheets
for (int i = 0; i < workbook.Worksheets.Count; i++)
{
Worksheet worksheet = workbook.Worksheets[i];
worksheet.Cells["A1"].PutValue("ID");
worksheet.Cells["B1"].PutValue("Name");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["B2"].PutValue("John");
worksheet.Cells["A3"].PutValue(2);
worksheet.Cells["B3"].PutValue("Jane");
}
// Create SqlScriptSaveOptions instance
SqlScriptSaveOptions options = new SqlScriptSaveOptions
{
TableName = "Employees",
CreateTable = true,
HasHeaderRow = true
};
// Display current SheetIndexes (null means all sheets)
Console.WriteLine("Initial SheetIndexes: " +
(options.SheetIndexes == null ? "All sheets" : string.Join(",", options.SheetIndexes)));
// Set SheetIndexes to export only first and third sheets (0 and 2)
options.SheetIndexes = new int[] { 0, 2 };
// Save with the options
workbook.Save("SqlScriptExportSelectedSheets.sql", options);
// Change SheetIndexes to export only the second sheet
options.SheetIndexes = new int[] { 1 };
workbook.Save("SqlScriptExportSecondSheet.sql", options);
// Set SheetIndexes to null to export all sheets
options.SheetIndexes = null;
workbook.Save("SqlScriptExportAllSheets.sql", options);
}
}
}
```
### See Also
* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)
