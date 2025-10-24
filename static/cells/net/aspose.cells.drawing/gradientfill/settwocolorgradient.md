##GradientFill.SetTwoColorGradient
GradientFill method. Sets the specified fill to a twocolor gradient. Only applies for Excel 2007
## SetTwoColorGradient(Color, Color, GradientStyleType, int) {#settwocolorgradient_1}
Sets the specified fill to a two-color gradient. Only applies for Excel 2007.
```csharp
public void SetTwoColorGradient(Color color1, Color color2, GradientStyleType style, int variant)
```
| Parameter | Type | Description |
| --- | --- | --- |
| color1 | Color | One gradient color. |
| color2 | Color | Two gradient color. |
| style | GradientStyleType | Gradient shading style. |
| variant | Int32 | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |
### See Also
* enum [GradientStyleType](../../gradientstyletype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
## SetTwoColorGradient(Color, double, Color, double, GradientStyleType, int) {#settwocolorgradient}
Sets the specified fill to a two-color gradient. Only applies for Excel 2007.
```csharp
public void SetTwoColorGradient(Color color1, double transparency1, Color color2,
double transparency2, GradientStyleType style, int variant)
```
| Parameter | Type | Description |
| --- | --- | --- |
| color1 | Color | One gradient color. |
| transparency1 | Double | The degree of transparency of the color1 as a value from 0.0 (opaque) through 1.0 (clear). |
| color2 | Color | Two gradient color. |
| transparency2 | Double | The degree of transparency of the color2 as a value from 0.0 (opaque) through 1.0 (clear). |
| style | GradientStyleType | Gradient shading style. |
| variant | Int32 | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |
### See Also
* enum [GradientStyleType](../../gradientstyletype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
