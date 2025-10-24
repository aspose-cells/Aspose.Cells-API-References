##set_one_color_gradient method
## set_one_color_gradient(self, color, degree, style, variant) {#aspose.pydrawing.Color-float-aspose.cells.drawing.GradientStyleType-int}
Sets the specified fill to a one-color gradient.
Only applies for Excel 2007.
```python
def set_one_color_gradient(self, color, degree, style, variant):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| color | aspose.pydrawing.Color | One gradient color. |
| degree | float | The gradient degree. Can be a value from 0.0 (dark) through 1.0 (light). |
| style | aspose.cells.drawing.GradientStyleType | Gradient shading style. |
| variant | int | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`GradientFill`](/cells/python-net/aspose.cells.drawing/gradientfill)
