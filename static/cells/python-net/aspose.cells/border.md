##Border class
## Border class
Encapsulates the object that represents the cell border.
The Border type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [theme_color](/cells/python-net/aspose.cells/border/theme_color) | Gets and sets the theme color of the border. |
| [color](/cells/python-net/aspose.cells/border/color) | Gets or sets the Color of the border. |
| [argb_color](/cells/python-net/aspose.cells/border/argb_color) | Gets and sets the color with a 32-bit ARGB value. |
| [line_style](/cells/python-net/aspose.cells/border/line_style) | Gets or sets the cell border type. |
### Example
```python
from aspose.cells import BorderType, CellBorderType, Workbook
from aspose.pydrawing import Color
workbook = Workbook()
sheets = workbook.worksheets
cell = sheets[0].cells.get("A1")
style = cell.get_style()
# Set top border style and color
border = style.borders.get(BorderType.TOP_BORDER)
border.line_style = CellBorderType.MEDIUM
border.color = Color.red
cell.set_style(style)
```
### See Also
* module [`aspose.cells`](..)
