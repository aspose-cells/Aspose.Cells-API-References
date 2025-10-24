##LineFormat Class
'LineFormat class. Encapsulates the object that represents lineformat in Go.'
## LineFormat class
Represents all setting of the line.
```go
type LineFormat struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewLineFormat](./newlineformat/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetHashCode](./gethashcode/) | Gets the hash code. |
|[Equals](./equals/) | Determines whether this instance has the same value as another specified LineFormat object. |
|[GetCompoundType](./getcompoundtype/) | Specifies the line compound type. |
|[SetCompoundType](./setcompoundtype/) | Specifies the line compound type. |
|[GetDashStyle](./getdashstyle/) | Specifies the line dash type. |
|[SetDashStyle](./setdashstyle/) | Specifies the line dash type. |
|[GetCapType](./getcaptype/) | Specifies the ending caps. |
|[SetCapType](./setcaptype/) | Specifies the ending caps. |
|[GetJoinType](./getjointype/) | Specifies the line join type. |
|[SetJoinType](./setjointype/) | Specifies the line join type. |
|[GetBeginArrowheadStyle](./getbeginarrowheadstyle/) | Gets and sets the begin arrow type of the line. |
|[SetBeginArrowheadStyle](./setbeginarrowheadstyle/) | Gets and sets the begin arrow type of the line. |
|[GetBeginArrowheadWidth](./getbeginarrowheadwidth/) | Gets and sets the begin arrow width type of the line. |
|[SetBeginArrowheadWidth](./setbeginarrowheadwidth/) | Gets and sets the begin arrow width type of the line. |
|[GetBeginArrowheadLength](./getbeginarrowheadlength/) | Gets and sets the begin arrow length type of the line. |
|[SetBeginArrowheadLength](./setbeginarrowheadlength/) | Gets and sets the begin arrow length type of the line. |
|[GetEndArrowheadStyle](./getendarrowheadstyle/) | Gets and sets the end arrow type of the line. |
|[SetEndArrowheadStyle](./setendarrowheadstyle/) | Gets and sets the end arrow type of the line. |
|[GetEndArrowheadWidth](./getendarrowheadwidth/) | Gets and sets the end arrow width type of the line. |
|[SetEndArrowheadWidth](./setendarrowheadwidth/) | Gets and sets the end arrow width type of the line. |
|[GetEndArrowheadLength](./getendarrowheadlength/) | Gets and sets the end arrow length type of the line. |
|[SetEndArrowheadLength](./setendarrowheadlength/) | Gets and sets the end arrow length type of the line. |
|[GetWeight](./getweight/) | Gets or sets the weight of the line in unit of points. |
|[SetWeight](./setweight/) | Gets or sets the weight of the line in unit of points. |
|[GetFillType](./getfilltype/) | Gets and sets fill type |
|[SetFillType](./setfilltype/) | Gets and sets fill type |
|[GetTransparency](./gettransparency/) | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
|[SetTransparency](./settransparency/) | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
|[GetGradientFill](./getgradientfill/) | Gets GradientFill object. |
|[GetTextureFill](./gettexturefill/) | Gets TextureFill object. |
|[GetSolidFill](./getsolidfill/) | Gets SolidFill object. |
|[GetPatternFill](./getpatternfill/) | Gets PatternFill object. |
|[GetGradientColorType](./getgradientcolortype/) | Returns the gradient color type for the specified fill. |
|[GetGradientStyle](./getgradientstyle/) | Returns the gradient style for the specified fill. |
|[GetGradientColor1](./getgradientcolor1/) | Returns the gradient color 1 for the specified fill. |
|[GetGradientColor2](./getgradientcolor2/) | Returns the gradient color 2 for the specified fill. |
|[GetGradientDegree](./getgradientdegree/) | Returns the gradient degree for the specified fill.Only applies for Excel 2007. |
|[GetGradientVariant](./getgradientvariant/) | Returns the gradient variant for the specified fill.Only applies for Excel 2007. |
|[GetPresetColor](./getpresetcolor/) | Returns the gradient preset color for the specified fill. |
|[SetOneColorGradient](./setonecolorgradient/) | Sets the specified fill to a one-color gradient.Only applies for Excel 2007. |
|[SetTwoColorGradient_Color_Color_GradientStyleType_Int](./settwocolorgradient_color_color_gradientstyletype_int/) | Sets the specified fill to a two-color gradient.Only applies for Excel 2007. |
|[SetTwoColorGradient_Color_Double_Color_Double_GradientStyleType_Int](./settwocolorgradient_color_double_color_double_gradientstyletype_int/) | Sets the specified fill to a two-color gradient.Only applies for Excel 2007. |
|[SetPresetColorGradient](./setpresetcolorgradient/) | Sets the specified fill to a preset-color gradient.Only applies for Excel 2007. |
|[GetTexture](./gettexture/) | Represents the texture type for the specified fill. |
|[SetTexture](./settexture/) | Represents the texture type for the specified fill. |
|[GetPattern](./getpattern/) | Represents an area's display pattern. |
|[SetPattern](./setpattern/) | Represents an area's display pattern. |
|[GetPictureFormatType](./getpictureformattype/) | Gets and sets the picture format type. |
|[SetPictureFormatType](./setpictureformattype/) | Gets and sets the picture format type. |
|[GetScale](./getscale/) | Gets and sets the picture format scale. |
|[SetScale](./setscale/) | Gets and sets the picture format scale. |
|[GetImageData](./getimagedata/) | Gets and sets the picture image data. |
|[SetImageData](./setimagedata/) | Gets and sets the picture image data. |
