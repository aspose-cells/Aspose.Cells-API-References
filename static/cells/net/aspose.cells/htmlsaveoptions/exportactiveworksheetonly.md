##HtmlSaveOptions.ExportActiveWorksheetOnly
HtmlSaveOptions property. Indicates if only exporting the active worksheet to html file. If true then only the active worksheet will be exported to html file If false then the whole workbook will be exported to html file. The default value is false
## HtmlSaveOptions.ExportActiveWorksheetOnly property
Indicates if only exporting the active worksheet to html file. If true then only the active worksheet will be exported to html file; If false then the whole workbook will be exported to html file. The default value is false.
```csharp
public bool ExportActiveWorksheetOnly { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyExportActiveWorksheetOnlyDemo
{
public static void Run()
{
// Create a new workbook with two worksheets
Workbook workbook = new Workbook();
workbook.Worksheets.Add("Sheet2");
// Add sample data to both sheets
workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
workbook.Worksheets[1].Cells["A1"].PutValue("Sheet2 Data");
// Set HTML save options to export only active worksheet
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
saveOptions.ExportActiveWorksheetOnly = true;
// Set first worksheet as active
workbook.Worksheets.ActiveSheetIndex = 0;
// Save with active worksheet only
workbook.Save("output_active_sheet_only.html", saveOptions);
// Change active sheet and save again
workbook.Worksheets.ActiveSheetIndex = 1;
workbook.Save("output_active_sheet_only2.html", saveOptions);
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
