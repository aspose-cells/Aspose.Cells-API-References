##ThemeColor class
## ThemeColor class
Represents a theme color.
The ThemeColor type exposes the following members:
### Constructors
| Constructor | Description |
| :- | :- |
| [`__init__(self, type, tint)`](/cells/python-net/aspose.cells/themecolor/__init__/#aspose.cells.themecolortype-float) |  |
### Properties
| Property | Description |
| :- | :- |
| [color_type](/cells/python-net/aspose.cells/themecolor/color_type) | Gets and sets the theme type. |
| [tint](/cells/python-net/aspose.cells/themecolor/tint) | Gets and sets the tint value. |
### Example
```python
from aspose.cells import BackgroundType, ThemeColor, ThemeColorType, Workbook
# Instantiating a Workbook object
workbook = Workbook()
cells = workbook.worksheets[0].cells
cells.get("A1").put_value("Hello World")
style = cells.get("A1").get_style()
# Set ThemeColorType.Text2 color type with 40% lighten as the font color.
style.font.theme_color = ThemeColor(ThemeColorType.TEXT2, 0.4)
style.pattern = BackgroundType.SOLID
# Set ThemeColorType.Background2 color type with 75% darken as the foreground color
style.foreground_theme_color = ThemeColor(ThemeColorType.BACKGROUND2, -0.75)
cells.get("A1").set_style(style)
# Saving the Excel file
workbook.save("book1.xlsx")
```
### See Also
* module [`aspose.cells`](..)
