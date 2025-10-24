##ImageOrPrintOptions.TextRenderingHint
ImageOrPrintOptions property. Specifies the quality of text rendering. The default value is TextRenderingHint.SystemDefault
## ImageOrPrintOptions.TextRenderingHint property
Specifies the quality of text rendering. The default value is TextRenderingHint.SystemDefault
```csharp
public TextRenderingHint TextRenderingHint { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing.Text;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ImageOrPrintOptionsPropertyTextRenderingHintDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample text to demonstrate text rendering
worksheet.Cells["A1"].PutValue("Text Rendering Hint Demo");
HtmlSaveOptions options = new HtmlSaveOptions();
#if !NETCOREAPP3_1_OR_GREATER
options.ImageOptions.TextRenderingHint = TextRenderingHint.AntiAlias;
#endif
workbook.Save("output.html", options);
}
}
}
```
### See Also
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
