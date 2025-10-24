##HtmlSaveOptions.ExportHeadings
HtmlSaveOptions property. Indicates whether exports sheets row and column headings when saving to HTML files
## HtmlSaveOptions.ExportHeadings property
Indicates whether exports sheet's row and column headings when saving to HTML files.
```csharp
[Obsolete("Use HtmlSaveOptions.ExportRowColumnHeadings instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ExportHeadings { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use HtmlSaveOptions.ExportRowColumnHeadings property. This property will be removed 12 months later since June 2022. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyExportHeadingsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Header1");
worksheet.Cells["B1"].PutValue("Header2");
worksheet.Cells["A2"].PutValue("Data1");
worksheet.Cells["B2"].PutValue("Data2");
// Create HTML save options and enable export headings
HtmlSaveOptions options = new HtmlSaveOptions();
options.ExportHeadings = true;
// Save as HTML with headings
workbook.Save("output_with_headings.html", options);
// Save again without headings for comparison
options.ExportHeadings = false;
workbook.Save("output_without_headings.html", options);
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
