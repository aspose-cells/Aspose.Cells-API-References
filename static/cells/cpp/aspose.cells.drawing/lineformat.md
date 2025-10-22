##Aspose::Cells::Drawing::LineFormat class
'Aspose::Cells::Drawing::LineFormat class. Represents all setting of the line in C++.'
## LineFormat class
Represents all setting of the line.
```cpp
class LineFormat : public Aspose::Cells::Drawing::FillFormat
```
## Methods
| Method | Description |
| --- | --- |
| [Equals(const Aspose::Cells::Object\& obj)](./equals/) | Determines whether this instance has the same value as another specified [LineFormat](./) object. |
| [FillFormat(FillFormat_Impl* impl)](../fillformat/fillformat/) | Constructs from an implementation object. |
| [FillFormat(const FillFormat\& src)](../fillformat/fillformat/) | Copy constructor. |
| [GetBeginArrowheadLength()](./getbeginarrowheadlength/) | Gets and sets the begin arrow length type of the line. |
| [GetBeginArrowheadStyle()](./getbeginarrowheadstyle/) | Gets and sets the begin arrow type of the line. |
| [GetBeginArrowheadWidth()](./getbeginarrowheadwidth/) | Gets and sets the begin arrow width type of the line. |
| [GetCapType()](./getcaptype/) | Specifies the ending caps. |
| [GetCompoundType()](./getcompoundtype/) | Specifies the line compound type. |
| [GetDashStyle()](./getdashstyle/) | Specifies the line dash type. |
| [GetEndArrowheadLength()](./getendarrowheadlength/) | Gets and sets the end arrow length type of the line. |
| [GetEndArrowheadStyle()](./getendarrowheadstyle/) | Gets and sets the end arrow type of the line. |
| [GetEndArrowheadWidth()](./getendarrowheadwidth/) | Gets and sets the end arrow width type of the line. |
| [GetFillType()](../fillformat/getfilltype/) | Gets and sets fill type. |
| [GetGradientColor1()](../fillformat/getgradientcolor1/) | Returns the gradient color 1 for the specified fill. |
| [GetGradientColor2()](../fillformat/getgradientcolor2/) | Returns the gradient color 2 for the specified fill. |
| [GetGradientColorType()](../fillformat/getgradientcolortype/) | Returns the gradient color type for the specified fill. |
| [GetGradientDegree()](../fillformat/getgradientdegree/) | Returns the gradient degree for the specified fill. Only applies for Excel 2007. |
| [GetGradientFill()](../fillformat/getgradientfill/) | Gets [GradientFill](../gradientfill/) object. |
| [GetGradientStyle()](../fillformat/getgradientstyle/) | Returns the gradient style for the specified fill. |
| [GetGradientVariant()](../fillformat/getgradientvariant/) | Returns the gradient variant for the specified fill. Only applies for Excel 2007. |
| [GetHashCode()](./gethashcode/) | Gets the hash code. |
| [GetImageData()](../fillformat/getimagedata/) | Gets and sets the picture image data. |
| [GetJoinType()](./getjointype/) | Specifies the line join type. |
| [GetPattern()](../fillformat/getpattern/) | Represents an area's display pattern. |
| [GetPatternFill()](../fillformat/getpatternfill/) | Gets [PatternFill](../patternfill/) object. |
| [GetPictureFormatType()](../fillformat/getpictureformattype/) | Gets and sets the picture format type. |
| [GetPresetColor()](../fillformat/getpresetcolor/) | Returns the gradient preset color for the specified fill. |
| [GetScale()](../fillformat/getscale/) | Gets and sets the picture format scale. |
| [GetSolidFill()](../fillformat/getsolidfill/) | Gets [SolidFill](../solidfill/) object. |
| [GetTexture()](../fillformat/gettexture/) | Represents the texture type for the specified fill. |
| [GetTextureFill()](../fillformat/gettexturefill/) | Gets [TextureFill](../texturefill/) object. |
| [GetTransparency()](../fillformat/gettransparency/) | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [GetWeight()](./getweight/) | Gets or sets the weight of the line in unit of points. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [LineFormat(LineFormat_Impl* impl)](./lineformat/) | Constructs from an implementation object. |
| [LineFormat(const LineFormat\& src)](./lineformat/) | Copy constructor. |
| [LineFormat(const FillFormat\& src)](./lineformat/) | Constructs from a parent object. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const LineFormat\& src)](./operator_asm/) | operator= |
| [operator=(const FillFormat\& src)](../fillformat/operator_asm/) | operator= |
| [SetBeginArrowheadLength(MsoArrowheadLength value)](./setbeginarrowheadlength/) | Gets and sets the begin arrow length type of the line. |
| [SetBeginArrowheadStyle(MsoArrowheadStyle value)](./setbeginarrowheadstyle/) | Gets and sets the begin arrow type of the line. |
| [SetBeginArrowheadWidth(MsoArrowheadWidth value)](./setbeginarrowheadwidth/) | Gets and sets the begin arrow width type of the line. |
| [SetCapType(LineCapType value)](./setcaptype/) | Specifies the ending caps. |
| [SetCompoundType(MsoLineStyle value)](./setcompoundtype/) | Specifies the line compound type. |
| [SetDashStyle(MsoLineDashStyle value)](./setdashstyle/) | Specifies the line dash type. |
| [SetEndArrowheadLength(MsoArrowheadLength value)](./setendarrowheadlength/) | Gets and sets the end arrow length type of the line. |
| [SetEndArrowheadStyle(MsoArrowheadStyle value)](./setendarrowheadstyle/) | Gets and sets the end arrow type of the line. |
| [SetEndArrowheadWidth(MsoArrowheadWidth value)](./setendarrowheadwidth/) | Gets and sets the end arrow width type of the line. |
| [SetFillType(FillType value)](../fillformat/setfilltype/) | Gets and sets fill type. |
| [SetImageData(const Vector \<uint8_t\>\& value)](../fillformat/setimagedata/) | Gets and sets the picture image data. |
| [SetJoinType(LineJoinType value)](./setjointype/) | Specifies the line join type. |
| [SetOneColorGradient(const Aspose::Cells::Color\& color, double degree, GradientStyleType style, int32_t variant)](../fillformat/setonecolorgradient/) | Sets the specified fill to a one-color gradient. Only applies for Excel 2007. |
| [SetPattern(FillPattern value)](../fillformat/setpattern/) | Represents an area's display pattern. |
| [SetPictureFormatType(FillPictureType value)](../fillformat/setpictureformattype/) | Gets and sets the picture format type. |
| [SetPresetColorGradient(GradientPresetType presetColor, GradientStyleType style, int32_t variant)](../fillformat/setpresetcolorgradient/) | Sets the specified fill to a preset-color gradient. Only applies for Excel 2007. |
| [SetScale(double value)](../fillformat/setscale/) | Gets and sets the picture format scale. |
| [SetTexture(TextureType value)](../fillformat/settexture/) | Represents the texture type for the specified fill. |
| [SetTransparency(double value)](../fillformat/settransparency/) | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [SetTwoColorGradient(const Aspose::Cells::Color\& color1, const Aspose::Cells::Color\& color2, GradientStyleType style, int32_t variant)](../fillformat/settwocolorgradient/) | Sets the specified fill to a two-color gradient. Only applies for Excel 2007. |
| [SetTwoColorGradient(const Aspose::Cells::Color\& color1, double transparency1, const Aspose::Cells::Color\& color2, double transparency2, GradientStyleType style, int32_t variant)](../fillformat/settwocolorgradient/) | Sets the specified fill to a two-color gradient. Only applies for Excel 2007. |
| [SetWeight(double value)](./setweight/) | Gets or sets the weight of the line in unit of points. |
| [~FillFormat()](../fillformat/~fillformat/) | Destructor. |
| [~LineFormat()](./~lineformat/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook workbook;
ShapeCollection shapes = workbook.GetWorksheets().Get(0).GetShapes();
Shape shape = shapes.AddRectangle(1, 0, 1, 0, 50, 100);
LineFormat lineFmt = shape.GetLine();
Aspose::Cells::Cleanup();
```
## See Also
* Class [FillFormat](../fillformat/)
* Namespace [Aspose::Cells::Drawing](../)
* Library [Aspose.Cells for C++](../../)
