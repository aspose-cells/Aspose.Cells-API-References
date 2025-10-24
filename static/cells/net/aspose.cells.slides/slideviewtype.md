##Enum SlideViewType
Aspose.Cells.Slides.SlideViewType enum. Represents the type when exporting to slides
## SlideViewType enumeration
Represents the type when exporting to slides.
```csharp
public enum SlideViewType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| View | `0` | Exporting as view in MS Excel. |
| Print | `1` | Exporting as printing. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slides;
namespace AsposeCellsExamples
{
public class SlidesClassSlideViewTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Slide 1 Content");
worksheet.Cells["A2"].PutValue("This will appear in the exported slides");
// Configure PPTX save options with SlideViewType
PptxSaveOptions saveOptions = new PptxSaveOptions
{
ExportViewType = SlideViewType.Print,
OnePagePerSheet = true
};
// Save as PPTX
workbook.Save("SlidesViewTypeDemo.pptx", saveOptions);
Console.WriteLine("PPTX file created with SlideViewType.Print");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Slides](../../aspose.cells.slides/)
* assembly [Aspose.Cells](../../)
