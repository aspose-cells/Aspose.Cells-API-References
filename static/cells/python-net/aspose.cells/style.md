##Style class
## Style class
Represents display style of excel document,such as font,color,alignment,border,etc.
The Style object contains all style attributes (font, number format, alignment, and so on) as properties.
The Style type exposes the following members:
### Constructors
| Constructor | Description |
| :- | :- |
| [`__init__(self)`](/cells/python-net/aspose.cells/style/__init__/#) | Initializes a new instance of the [`Style`](/cells/python-net/aspose.cells/style) class. |
### Properties
| Property | Description |
| :- | :- |
| [background_theme_color](/cells/python-net/aspose.cells/style/background_theme_color) | Gets and sets the background theme color. |
| [foreground_theme_color](/cells/python-net/aspose.cells/style/foreground_theme_color) | Gets and sets the foreground theme color. |
| [name](/cells/python-net/aspose.cells/style/name) | Gets or sets the name of the style. |
| [pattern](/cells/python-net/aspose.cells/style/pattern) | Gets or sets the cell background pattern type. |
| [borders](/cells/python-net/aspose.cells/style/borders) | Gets the [`BorderCollection`](/cells/python-net/aspose.cells/bordercollection) of the style. |
| [background_color](/cells/python-net/aspose.cells/style/background_color) | Gets or sets a style's background color. |
| [background_argb_color](/cells/python-net/aspose.cells/style/background_argb_color) | Gets and sets the background color with a 32-bit ARGB value. |
| [foreground_color](/cells/python-net/aspose.cells/style/foreground_color) | Gets or sets a style's foreground color. |
| [foreground_argb_color](/cells/python-net/aspose.cells/style/foreground_argb_color) | Gets and sets the foreground color with a 32-bit ARGB value. |
| [has_borders](/cells/python-net/aspose.cells/style/has_borders) | Checks whether there are borders have been set for the style. |
| [parent_style](/cells/python-net/aspose.cells/style/parent_style) | Gets the parent style of this style. |
| [is_number_format_applied](/cells/python-net/aspose.cells/style/is_number_format_applied) | Indicate whether the number formatting should be applied. |
| [is_font_applied](/cells/python-net/aspose.cells/style/is_font_applied) | Indicate whether the font formatting should be applied. |
| [is_alignment_applied](/cells/python-net/aspose.cells/style/is_alignment_applied) | Indicate whether the alignment formatting should be applied. |
| [is_border_applied](/cells/python-net/aspose.cells/style/is_border_applied) | Indicate whether the border formatting should be applied. |
| [is_fill_applied](/cells/python-net/aspose.cells/style/is_fill_applied) | Indicate whether the fill formatting should be applied. |
| [is_protection_applied](/cells/python-net/aspose.cells/style/is_protection_applied) | Indicate whether the protection formatting should be applied. |
| [indent_level](/cells/python-net/aspose.cells/style/indent_level) | Represents the indent level for the cell or range. Can only be an integer from 0 to 250. |
| [font](/cells/python-net/aspose.cells/style/font) | Gets a [`Style.font`](/cells/python-net/aspose.cells/style#font) object. |
| [rotation_angle](/cells/python-net/aspose.cells/style/rotation_angle) | Represents text rotation angle. |
| [horizontal_alignment](/cells/python-net/aspose.cells/style/horizontal_alignment) | Gets or sets the horizontal alignment type of the text in a cell. |
| [vertical_alignment](/cells/python-net/aspose.cells/style/vertical_alignment) | Gets or sets the vertical alignment type of the text in a cell. |
| [is_text_wrapped](/cells/python-net/aspose.cells/style/is_text_wrapped) | Gets or sets a value indicating whether the text within a cell is wrapped. |
| [number](/cells/python-net/aspose.cells/style/number) | Gets or sets the display format of numbers and dates. The formatting patterns are different for different regions. |
| [is_locked](/cells/python-net/aspose.cells/style/is_locked) | Gets or sets a value indicating whether a cell can be modified or not. |
| [custom](/cells/python-net/aspose.cells/style/custom) | Represents the custom number format string of this style object.
| [culture_custom](/cells/python-net/aspose.cells/style/culture_custom) | Gets and sets the culture-dependent pattern string for number format.
| [invariant_custom](/cells/python-net/aspose.cells/style/invariant_custom) | Gets the culture-independent pattern string for number format.
| [is_formula_hidden](/cells/python-net/aspose.cells/style/is_formula_hidden) | Represents if the formula will be hidden when the worksheet is protected. |
| [shrink_to_fit](/cells/python-net/aspose.cells/style/shrink_to_fit) | Represents if text automatically shrinks to fit in the available column width. |
| [text_direction](/cells/python-net/aspose.cells/style/text_direction) | Represents text reading order. |
| [is_justify_distributed](/cells/python-net/aspose.cells/style/is_justify_distributed) | Indicates if the cells justified or distributed alignment should be used on the last line of text. |
| [quote_prefix](/cells/python-net/aspose.cells/style/quote_prefix) | Indicates whether the cell's value starts with single quote mark. |
| [is_gradient](/cells/python-net/aspose.cells/style/is_gradient) | Indicates whether the cell shading is a gradient pattern. |
| [is_percent](/cells/python-net/aspose.cells/style/is_percent) | Indicates whether the number format is a percent format. |
| [is_date_time](/cells/python-net/aspose.cells/style/is_date_time) | Indicates whether the number format is a date format. |
### Methods
| Method | Description |
| :- | :- |
| [`set_border(self, border_type, border_style, border_color)`](/cells/python-net/aspose.cells/style/set_border/#aspose.cells.bordertype-aspose.cells.cellbordertype-aspose.pydrawing.color) | Sets the borders of the style. |
| [`set_border(self, border_type, border_style, border_color)`](/cells/python-net/aspose.cells/style/set_border/#aspose.cells.bordertype-aspose.cells.cellbordertype-aspose.cells.cellscolor) | Sets the borders of the style. |
| [`set_pattern_color(self, pattern, color1, color2)`](/cells/python-net/aspose.cells/style/set_pattern_color/#aspose.cells.backgroundtype-aspose.pydrawing.color-aspose.pydrawing.color) | Sets the background color. |
| [`copy(self, style)`](/cells/python-net/aspose.cells/style/copy/#aspose.cells.style) | Copies data from another style object |
| [`update(self)`](/cells/python-net/aspose.cells/style/update/#) | Apply the named style to the styles of the cells which use this named style.
| [`is_modified(self, modify_flag)`](/cells/python-net/aspose.cells/style/is_modified/#aspose.cells.stylemodifyflag) | Checks whether the specified properties of the style have been modified.
| [`set_custom(self, custom, builtin_preference)`](/cells/python-net/aspose.cells/style/set_custom/#system.string-bool) | Sets the Custom number format string of a cell. |
| [`set_two_color_gradient(self, color1, color2, gradient_style_type, variant)`](/cells/python-net/aspose.cells/style/set_two_color_gradient/#aspose.pydrawing.color-aspose.pydrawing.color-aspose.cells.drawing.gradientstyletype-int) | Sets the specified fill to a two-color gradient. |
| [`get_two_color_gradient(self, color1, color2, gradient_style_type, variant)`](/cells/python-net/aspose.cells/style/get_two_color_gradient/#aspose.pydrawing.color&-aspose.pydrawing.color&-any-any) | Get the two-color gradient setting. |
| [`get_two_color_gradient_setting(self)`](/cells/python-net/aspose.cells/style/get_two_color_gradient_setting/#) | Get the two-color gradient setting. |
| [`to_json(self)`](/cells/python-net/aspose.cells/style/to_json/#) | Convert [`Style`](/cells/python-net/aspose.cells/style) to JSON struct data. |
### Example
```python
from aspose.cells import Workbook
from aspose.pydrawing import Color
workbook = Workbook()
sheets = workbook.worksheets
cell = sheets[0].cells.get("A1")
style = cell.get_style()
style.font.name = "Times New Roman"
style.font.color = Color.blue
cell.set_style(style)
```
### See Also
* module [`aspose.cells`](..)
* class [`BorderCollection`](/cells/python-net/aspose.cells/bordercollection)
* class [`Style`](/cells/python-net/aspose.cells/style)
