##HtmlSaveOptions.DefaultFontName
HtmlSaveOptions property. Specify the default font name for exporting html the default font will be used when the font of style is not existing If this property is null Aspose.Cells will use universal font which have the same family with the original font the default value is null
## HtmlSaveOptions.DefaultFontName property
Specify the default font name for exporting html, the default font will be used when the font of style is not existing, If this property is null, Aspose.Cells will use universal font which have the same family with the original font, the default value is null.
```csharp
public string DefaultFontName { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyDefaultFontNameDemo
{
public static void Run()
{
// Create a sample workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Sample Text");
// Set HTML save options with custom default font
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
saveOptions.DefaultFontName = "Courier New";
// Save to HTML with the specified font
workbook.Save("output.html", saveOptions);
Console.WriteLine("HTML file saved with default font: " + saveOptions.DefaultFontName);
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
