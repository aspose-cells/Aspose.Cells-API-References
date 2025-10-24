##GradientFill Class
'GradientFill class. Encapsulates the object that represents gradientfill in Go.'
## GradientFill class
Represents the gradient fill.
```go
type GradientFill struct  {
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
|[GetGradientStops](./getgradientstops/) | Represents the gradient stop collection. |
|[SetGradient](./setgradient/) | Set the gradient fill type and direction. |
|[GetFillType](./getfilltype/) | Gets the gradient fill type. |
|[GetDirectionType](./getdirectiontype/) | Gets the gradient direction type. |
|[GetAngle](./getangle/) | The angle of linear fill. |
|[SetAngle](./setangle/) | The angle of linear fill. |
|[SetPresetThemeGradient](./setpresetthemegradient/) | Sets preset theme gradient fill. |
|[SetOneColorGradient](./setonecolorgradient/) | Sets the specified fill to a one-color gradient.Only applies for Excel 2007. |
|[SetTwoColorGradient_Color_Color_GradientStyleType_Int](./settwocolorgradient_color_color_gradientstyletype_int/) | Sets the specified fill to a two-color gradient.Only applies for Excel 2007. |
|[SetTwoColorGradient_Color_Double_Color_Double_GradientStyleType_Int](./settwocolorgradient_color_double_color_double_gradientstyletype_int/) | Sets the specified fill to a two-color gradient.Only applies for Excel 2007. |
