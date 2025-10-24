##HtmlSaveOptions.DisableCss
HtmlSaveOptions property. Indicates whether only inline styles are applied without relying on CSS. The default value is false
## HtmlSaveOptions.DisableCss property
Indicates whether only inline styles are applied, without relying on CSS. The default value is false.
```csharp
public bool DisableCss { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class HtmlSaveOptionsPropertyDisableCssDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data and formatting
worksheet.Cells["A1"].PutValue("Sample Data");
worksheet.Cells["A1"].GetStyle().Font.IsBold = true;
worksheet.Cells["A1"].GetStyle().Font.Color = System.Drawing.Color.Red;
worksheet.Cells["B1"].PutValue("Formatted Cell");
worksheet.Cells["B1"].GetStyle().Font.IsItalic = true;
worksheet.Cells["B1"].GetStyle().Font.Underline = FontUnderlineType.Single;
// Create HtmlSaveOptions instance
HtmlSaveOptions options = new HtmlSaveOptions();
// Display current DisableCss value
Console.WriteLine("Current DisableCss value: " + options.DisableCss);
// Set DisableCss to true (using inline styles instead of CSS)
options.DisableCss = true;
workbook.Save("HtmlWithInlineStyles.html", options);
// Set DisableCss to false (using CSS styles)
options.DisableCss = false;
workbook.Save("HtmlWithCssStyles.html", options);
// Compare the output files to see the difference in styling approach
Console.WriteLine("Files saved with different DisableCss settings.");
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
