##Range.ToHtml
Range method. Convert the range to html
## Range.ToHtml method
Convert the range to html .
```csharp
public byte[] ToHtml(HtmlSaveOptions saveOptions)
```
| Parameter | Type | Description |
| --- | --- | --- |
| saveOptions | HtmlSaveOptions | Options for coverting range to html. |
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangeMethodToHtmlWithHtmlSaveOptionsDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate some data in the range A1:J25
for (int i = 0; i < 25; i++)
{
for (int j = 0; j < 10; j++)
{
worksheet.Cells[i, j].Value = $"Cell {i+1},{j+1}";
}
}
// Create a range with fully qualified type name
Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:J25");
// Create HTML save options
HtmlSaveOptions options = new HtmlSaveOptions();
options.ExportImagesAsBase64 = true;
// Convert range to HTML
byte[] htmlData = range.ToHtml(options);
// Save HTML to file
File.WriteAllBytes("output.html", htmlData);
}
}
}
```
### See Also
* class [HtmlSaveOptions](../../htmlsaveoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
