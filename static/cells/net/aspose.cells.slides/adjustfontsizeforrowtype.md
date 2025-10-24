##Enum AdjustFontSizeForRowType
Aspose.Cells.Slides.AdjustFontSizeForRowType enum. Represents which kind of rows should be ajusted
## AdjustFontSizeForRowType enumeration
Represents which kind of rows should be ajusted.
```csharp
public enum AdjustFontSizeForRowType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | `0` | No adjsut. |
| EmptyRows | `1` | If the row is empty, change font size to fit row height. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slides;
namespace AsposeCellsExamples
{
public class SlidesClassAdjustFontSizeForRowTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Fill some data into the worksheet
worksheet.Cells["A1"].PutValue("Hello");
worksheet.Cells["A2"].PutValue("World");
// Create an instance of PptxSaveOptions with AdjustFontSizeForRowType setting
PptxSaveOptions saveOptions = new PptxSaveOptions
{
AdjustFontSizeForRowType = AdjustFontSizeForRowType.EmptyRows
};
// Save the workbook as a PPTX file
workbook.Save("AdjustFontSizeForRowTypeDemo.pptx", saveOptions);
}
}
}
```
### See Also
* namespace [Aspose.Cells.Slides](../../aspose.cells.slides/)
* assembly [Aspose.Cells](../../)
