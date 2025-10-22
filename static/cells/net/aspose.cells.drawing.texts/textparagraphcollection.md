##Class TextParagraphCollection
Aspose.Cells.Drawing.Texts.TextParagraphCollection class. Represents all text paragraph
## TextParagraphCollection class
Represents all text paragraph.
```csharp
public class TextParagraphCollection : IEnumerable
```
## Properties
| Name | Description |
| --- | --- |
| [Count](../../aspose.cells.drawing.texts/textparagraphcollection/count/) { get; } | Gets the count of text paragraphs. |
| [Item](../../aspose.cells.drawing.texts/textparagraphcollection/item/) { get; } | Gets the [`TextParagraph`](../textparagraph/) object at specific index. |
## Methods
| Name | Description |
| --- | --- |
| [GetEnumerator](../../aspose.cells.drawing.texts/textparagraphcollection/getenumerator/)() | Gets the enumerator of the paragraphs. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
namespace AsposeCellsExamples
{
public class TextsClassTextParagraphCollectionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a text box to the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
// Set multi-line text
shape.Text = "First paragraph\nSecond paragraph";
// Get the paragraph collection
TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
// Access and modify the second paragraph
TextParagraph secondParagraph = paragraphs[1];
secondParagraph.LineSpaceSizeType = LineSpaceSizeType.Points;
secondParagraph.LineSpace = 20;
secondParagraph.SpaceAfter = 30;
secondParagraph.SpaceBefore = 40;
// Save the workbook
workbook.Save("TextParagraphCollectionDemo.xlsx");
Console.WriteLine("Text paragraph formatting saved successfully.");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)
