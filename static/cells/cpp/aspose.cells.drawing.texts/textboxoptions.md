##Aspose::Cells::Drawing::Texts::TextBoxOptions class
'Aspose::Cells::Drawing::Texts::TextBoxOptions class. Represents the text options of the shape in C++.'
## TextBoxOptions class
Represents the text options of the shape.
```cpp
class TextBoxOptions
```
## Methods
| Method | Description |
| --- | --- |
| [GetAllowTextToOverflow()](./getallowtexttooverflow/) | Whether allow text to overflow shape. |
| [GetBottomMarginPt()](./getbottommarginpt/) | Returns the bottom margin in unit of Points. |
| [GetLeftMarginPt()](./getleftmarginpt/) | Gets and sets the left margin in unit of Points. |
| [GetResizeToFitText()](./getresizetofittext/) | Indicates whether to resize the shape to fit the text. |
| [GetRightMarginPt()](./getrightmarginpt/) | Gets and sets the right margin in unit of Points. |
| [GetShapeTextDirection()](./getshapetextdirection/) | Gets or sets the text display direction within a given text body. It corresponds to "Format Shape - Text Options - Text Box - Text direction" in Excel. |
| [GetShapeTextVerticalAlignment()](./getshapetextverticalalignment/) | It corresponds to "Format Shape - Text Options - Text Box - Vertical Alignment" in Excel. |
| [GetTopMarginPt()](./gettopmarginpt/) | Gets and sets the top margin in unit of Points. |
| [GetWrapTextInShape()](./getwraptextinshape/) | Specifies text wrapping within a shape. False - No wrapping will occur on text body. True - Wrapping will occur on text body. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const TextBoxOptions\& src)](./operator_asm/) | operator= |
| [SetAllowTextToOverflow(bool value)](./setallowtexttooverflow/) | Whether allow text to overflow shape. |
| [SetBottomMarginPt(double value)](./setbottommarginpt/) | Returns the bottom margin in unit of Points. |
| [SetLeftMarginPt(double value)](./setleftmarginpt/) | Gets and sets the left margin in unit of Points. |
| [SetResizeToFitText(bool value)](./setresizetofittext/) | Indicates whether to resize the shape to fit the text. |
| [SetRightMarginPt(double value)](./setrightmarginpt/) | Gets and sets the right margin in unit of Points. |
| [SetShapeTextDirection(TextVerticalType value)](./setshapetextdirection/) | Gets or sets the text display direction within a given text body. It corresponds to "Format Shape - Text Options - Text Box - Text direction" in Excel. |
| [SetShapeTextVerticalAlignment(ShapeTextVerticalAlignmentType value)](./setshapetextverticalalignment/) | It corresponds to "Format Shape - Text Options - Text Box - Vertical Alignment" in Excel. |
| [SetTopMarginPt(double value)](./settopmarginpt/) | Gets and sets the top margin in unit of Points. |
| [SetWrapTextInShape(bool value)](./setwraptextinshape/) | Specifies text wrapping within a shape. False - No wrapping will occur on text body. True - Wrapping will occur on text body. |
| [TextBoxOptions(TextBoxOptions_Impl* impl)](./textboxoptions/) | Constructs from an implementation object. |
| [TextBoxOptions(const TextBoxOptions\& src)](./textboxoptions/) | Copy constructor. |
| [~TextBoxOptions()](./~textboxoptions/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook workbook;
int index = workbook.GetWorksheets().Get(0).GetTextBoxes().Add(0, 0, 350, 350);
Shape shape = workbook.GetWorksheets().Get(0).GetTextBoxes().Get(index);
shape.SetText(u"This is test.");
//Save the excel file.
workbook.Save("exmaple.xlsx");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells::Drawing::Texts](../)
* Library [Aspose.Cells for C++](../../)
