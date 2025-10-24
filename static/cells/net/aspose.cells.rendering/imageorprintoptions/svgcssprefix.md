##ImageOrPrintOptions.SvgCssPrefix
ImageOrPrintOptions property. Gets and sets the prefix of the css name in svgthe default value is empty string
## ImageOrPrintOptions.SvgCssPrefix property
Gets and sets the prefix of the css name in svg,the default value is empty string.
```csharp
[Obsolete("Use SvgImageOptions.CssPrefix property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string SvgCssPrefix { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use [`CssPrefix`](../../svgimageoptions/cssprefix/). This property will be removed 12 months later since April 2025. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class ImageOrPrintOptionsPropertySvgCssPrefixDemo
{
public static void Run()
{
string prefix = "custom_prefix_";
Workbook workbook = new Workbook();
workbook.Worksheets[0].Cells["A1"].PutValue("SVG CSS Prefix Test");
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.ImageType = Aspose.Cells.Drawing.ImageType.Svg;
options.OnePagePerSheet = true;
options.SvgCssPrefix = prefix;
SheetRender renderer = new SheetRender(workbook.Worksheets[0], options);
using (MemoryStream stream = new MemoryStream())
{
renderer.ToImage(0, stream);
stream.Position = 0;
using (StreamReader reader = new StreamReader(stream))
{
string svgContent = reader.ReadToEnd();
Console.WriteLine("SVG contains CSS prefix: " + svgContent.Contains(prefix + "f"));
}
}
}
}
}
```
### See Also
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
