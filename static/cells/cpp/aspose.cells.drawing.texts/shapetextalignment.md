##Aspose::Cells::Drawing::Texts::ShapeTextAlignment class
'Aspose::Cells::Drawing::Texts::ShapeTextAlignment class. Represents the setting of shape''s text alignment; in C++.'
## ShapeTextAlignment class
Represents the setting of shape's text alignment;.
```cpp
class ShapeTextAlignment
```
## Methods
| Method | Description |
| --- | --- |
| [Equals(const Aspose::Cells::Object\& obj)](./equals/) | Determines whether this instance has the same value as another specified [ShapeTextAlignment](./) object. |
| [GetAutoSize()](./getautosize/) | Indicates if size of shape is adjusted automatically according to its content. |
| [GetBottomMarginPt()](./getbottommarginpt/) | Returns the bottom margin in unit of Points. |
| [GetHashCode()](./gethashcode/) |  |
| [GetLeftMarginPt()](./getleftmarginpt/) | Returns the left margin in unit of Points. |
| [GetNumberOfColumns()](./getnumberofcolumns/) | Gets and sets the number of columns of text in the bounding rectangle. |
| [GetRightMarginPt()](./getrightmarginpt/) | Returns the right margin in unit of Points. |
| [GetRotateTextWithShape()](./getrotatetextwithshape/) | Indicates whether rotating text with shape. |
| [GetRotationAngle()](./getrotationangle/) | Gets and sets the rotation of the shape. |
| [GetTextHorizontalOverflow()](./gettexthorizontaloverflow/) | Gets and sets the text horizontal overflow type of the text box. |
| [GetTextShapeType()](./gettextshapetype/) | Gets and set the transform type of text. |
| [GetTextVerticalOverflow()](./gettextverticaloverflow/) | Gets and sets the text vertical overflow type of the text box. |
| [GetTextVerticalType()](./gettextverticaltype/) | Gets and sets the text direction. |
| [GetTopMarginPt()](./gettopmarginpt/) | Returns the top margin in unit of Points. |
| [IsAutoMargin()](./isautomargin/) | Indicates whether the margin of the text frame is automatic. |
| [IsLockedText()](./islockedtext/) | Indicates whether the shape is locked when worksheet is protected. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsTextWrapped()](./istextwrapped/) | Gets or sets the text wrapped type of the shape which contains text. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ShapeTextAlignment\& src)](./operator_asm/) | operator= |
| [SetAutoSize(bool value)](./setautosize/) | Indicates if size of shape is adjusted automatically according to its content. |
| [SetBottomMarginPt(double value)](./setbottommarginpt/) | Returns the bottom margin in unit of Points. |
| [SetIsAutoMargin(bool value)](./setisautomargin/) | Indicates whether the margin of the text frame is automatic. |
| [SetIsLockedText(bool value)](./setislockedtext/) | Indicates whether the shape is locked when worksheet is protected. |
| [SetIsTextWrapped(bool value)](./setistextwrapped/) | Gets or sets the text wrapped type of the shape which contains text. |
| [SetLeftMarginPt(double value)](./setleftmarginpt/) | Returns the left margin in unit of Points. |
| [SetNumberOfColumns(int32_t value)](./setnumberofcolumns/) | Gets and sets the number of columns of text in the bounding rectangle. |
| [SetRightMarginPt(double value)](./setrightmarginpt/) | Returns the right margin in unit of Points. |
| [SetRotateTextWithShape(bool value)](./setrotatetextwithshape/) | Indicates whether rotating text with shape. |
| [SetRotationAngle(double value)](./setrotationangle/) | Gets and sets the rotation of the shape. |
| [SetTextHorizontalOverflow(TextOverflowType value)](./settexthorizontaloverflow/) | Gets and sets the text horizontal overflow type of the text box. |
| [SetTextShapeType(AutoShapeType value)](./settextshapetype/) | Gets and set the transform type of text. |
| [SetTextVerticalOverflow(TextOverflowType value)](./settextverticaloverflow/) | Gets and sets the text vertical overflow type of the text box. |
| [SetTextVerticalType(TextVerticalType value)](./settextverticaltype/) | Gets and sets the text direction. |
| [SetTopMarginPt(double value)](./settopmarginpt/) | Returns the top margin in unit of Points. |
| [ShapeTextAlignment(ShapeTextAlignment_Impl* impl)](./shapetextalignment/) | Constructs from an implementation object. |
| [ShapeTextAlignment(const ShapeTextAlignment\& src)](./shapetextalignment/) | Copy constructor. |
| [~ShapeTextAlignment()](./~shapetextalignment/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook workbook;
Shape shape = workbook.GetWorksheets().Get(0).GetShapes().AddRectangle(1, 0, 1, 0, 50, 100);
ShapeTextAlignment shapeTextAlignment = shape.GetTextBody().GetTextAlignment();
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells::Drawing::Texts](../)
* Library [Aspose.Cells for C++](../../)
