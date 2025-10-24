##Class TextBoxOptions
Aspose.Cells.Drawing.Texts.TextBoxOptions class. Represents the text options of the shape
## TextBoxOptions class
Represents the text options of the shape
```csharp
public class TextBoxOptions
```
## Properties
| Name | Description |
| --- | --- |
| [AllowTextToOverflow](../../aspose.cells.drawing.texts/textboxoptions/allowtexttooverflow/) { get; set; } | Whether allow text to overflow shape. |
| [BottomMarginPt](../../aspose.cells.drawing.texts/textboxoptions/bottommarginpt/) { get; set; } | Returns the bottom margin in unit of Points |
| [LeftMarginPt](../../aspose.cells.drawing.texts/textboxoptions/leftmarginpt/) { get; set; } | Gets and sets the left margin in unit of Points. |
| [ResizeToFitText](../../aspose.cells.drawing.texts/textboxoptions/resizetofittext/) { get; set; } | Indicates whether to resize the shape to fit the text |
| [RightMarginPt](../../aspose.cells.drawing.texts/textboxoptions/rightmarginpt/) { get; set; } | Gets and sets the right margin in unit of Points. |
| [ShapeTextDirection](../../aspose.cells.drawing.texts/textboxoptions/shapetextdirection/) { get; set; } | Gets or sets the text display direction within a given text body. It corresponds to "Format Shape - Text Options - Text Box - Text direction" in Excel |
| [ShapeTextVerticalAlignment](../../aspose.cells.drawing.texts/textboxoptions/shapetextverticalalignment/) { get; set; } | It corresponds to "Format Shape - Text Options - Text Box - Vertical Alignment" in Excel. |
| [TopMarginPt](../../aspose.cells.drawing.texts/textboxoptions/topmarginpt/) { get; set; } | Gets and sets the top margin in unit of Points. |
| [WrapTextInShape](../../aspose.cells.drawing.texts/textboxoptions/wraptextinshape/) { get; set; } | Specifies text wrapping within a shape. False - No wrapping will occur on text body. True - Wrapping will occur on text body. |
### Examples
```csharp
[C#]
//Instantiating a Workbook object
Workbook workbook = new Workbook();
int index = workbook.Worksheets[0].TextBoxes.Add(0, 0, 350, 350);
Shape shape = workbook.Worksheets[0].TextBoxes[index];
shape.Text = "This is test.";
//do your business
//Save the excel file.
workbook.Save("exmaple.xlsx");
```
### See Also
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)
