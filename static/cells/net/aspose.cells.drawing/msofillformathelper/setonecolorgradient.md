##MsoFillFormatHelper.SetOneColorGradient
MsoFillFormatHelper method. Sets the specified fill to a onecolor gradient
## MsoFillFormatHelper.SetOneColorGradient method
Sets the specified fill to a one-color gradient.
```csharp
public void SetOneColorGradient(Color color, double degree, GradientStyleType style, int variant)
```
| Parameter | Type | Description |
| --- | --- | --- |
| color | Color | One gradient color. |
| degree | Double | The gradient degree. Can be a value from 0.0 (dark) through 1.0 (light). |
| style | GradientStyleType | Gradient shading style. |
| variant | Int32 | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |
### See Also
* enum [GradientStyleType](../../gradientstyletype/)
* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
