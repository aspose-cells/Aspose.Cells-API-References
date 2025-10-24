##FillFormat Class
'FillFormat class. Encapsulates the object that represents fillformat in Go.'
## FillFormat class
Encapsulates the object that represents fill formatting for a shape.
```go
type FillFormat struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
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
|[Equals](./equals/) |  |
|[GetHashCode](./gethashcode/) | Gets the hash code. |
