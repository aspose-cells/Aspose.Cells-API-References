##HtmlSaveOptions.ExportHiddenWorksheet
HtmlSaveOptions property. Indicating if exporting the hidden worksheet content.The default value is true
## HtmlSaveOptions.ExportHiddenWorksheet property
Indicating if exporting the hidden worksheet content.The default value is true.
```csharp
public bool ExportHiddenWorksheet { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyExportHiddenWorksheetDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet1 = workbook.Worksheets[0];
worksheet1.Name = "VisibleSheet";
worksheet1.Cells["A1"].PutValue("Visible Data");
Worksheet worksheet2 = workbook.Worksheets.Add("HiddenSheet");
worksheet2.Cells["A1"].PutValue("Hidden Data");
worksheet2.IsVisible = false;
// Set HTML save options
HtmlSaveOptions saveOptions = new HtmlSaveOptions
{
ExportHiddenWorksheet = false, // Don't export hidden worksheets
ExportActiveWorksheetOnly = false
};
// Save with hidden worksheet not exported
workbook.Save("output_without_hidden.html", saveOptions);
// Change option to export hidden worksheets
saveOptions.ExportHiddenWorksheet = true;
// Save with hidden worksheet exported
workbook.Save("output_with_hidden.html", saveOptions);
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
