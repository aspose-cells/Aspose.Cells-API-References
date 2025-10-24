##HtmlSaveOptions.ParseHtmlTagInCell
HtmlSaveOptions property. Indicates whether html tagsuch as div/div in cell should be parsed as cell value or preserved as it is. The default value is true
## HtmlSaveOptions.ParseHtmlTagInCell property
Indicates whether html tag(such as `<div></div>`) in cell should be parsed as cell value or preserved as it is. The default value is true.
```csharp
public bool ParseHtmlTagInCell { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyParseHtmlTagInCellDemo
{
public static void Run()
{
// Create a workbook with sample data containing HTML tags
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set cell value with HTML tags
worksheet.Cells["A1"].PutValue("<b>Bold Text</b> and <i>Italic Text</i>");
// Create HTML save options and enable HTML tag parsing
HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions(SaveFormat.Html);
htmlSaveOptions.ParseHtmlTagInCell = true;
// Save the workbook with HTML tags parsed
workbook.Save("output.html", htmlSaveOptions);
Console.WriteLine("HTML saved with ParseHtmlTagInCell enabled.");
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
