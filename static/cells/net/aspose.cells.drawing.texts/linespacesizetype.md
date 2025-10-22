##Enum LineSpaceSizeType
Aspose.Cells.Drawing.Texts.LineSpaceSizeType enum. Represents the unit type of line space size
## LineSpaceSizeType enumeration
Represents the unit type of line space size.
```csharp
public enum LineSpaceSizeType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Percentage | `0` | Represents in unit of a percentage of the text size. |
| Points | `1` | Represents in unit of points. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
namespace AsposeCellsExamples
{
public class TextsClassLineSpaceSizeTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box shape
Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
// Set text content
textBox.Text = "Sample Text\nSecond Line";
// Access the first paragraph of the text box
TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];
// Set space after size type to Points
paragraph.SpaceAfterSizeType = LineSpaceSizeType.Points;
// Set space after value (12 points)
paragraph.SpaceAfter = 12;
// Save the workbook
workbook.Save("output.xlsx");
Console.WriteLine("Text box with line spacing created successfully.");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)
