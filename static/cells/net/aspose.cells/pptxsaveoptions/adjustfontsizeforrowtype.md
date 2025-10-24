##PptxSaveOptions.AdjustFontSizeForRowType
PptxSaveOptions property. Represents what type of line needs to be adjusted size of font if height of row is small
## PptxSaveOptions.AdjustFontSizeForRowType property
Represents what type of line needs to be adjusted size of font if height of row is small.
```csharp
public AdjustFontSizeForRowType AdjustFontSizeForRowType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slides;
namespace AsposeCellsExamples
{
public class PptxSaveOptionsPropertyAdjustFontSizeForRowTypeDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data and empty rows
worksheet.Cells["A1"].PutValue("Header");
worksheet.Cells["A2"].PutValue("Data 1");
worksheet.Cells["A3"].PutValue(""); // Empty row
worksheet.Cells["A4"].PutValue("Data 2");
// Create PPTX save options
PptxSaveOptions saveOptions = new PptxSaveOptions();
saveOptions.AdjustFontSizeForRowType = AdjustFontSizeForRowType.EmptyRows;
// Save to PPTX
workbook.Save("output.pptx", saveOptions);
Console.WriteLine("File saved with AdjustFontSizeForRowType setting");
}
}
}
```
### See Also
* enum [AdjustFontSizeForRowType](../../../aspose.cells.slides/adjustfontsizeforrowtype/)
* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
