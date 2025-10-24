##Font class
## Font class
Encapsulates the font object used in a spreadsheet.
The Font type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [charset](/cells/python-net/aspose.cells/font/charset) | Represent the character set. |
| [is_italic](/cells/python-net/aspose.cells/font/is_italic) | Gets or sets a value indicating whether the font is italic. |
| [is_bold](/cells/python-net/aspose.cells/font/is_bold) | Gets or sets a value indicating whether the font is bold. |
| [caps_type](/cells/python-net/aspose.cells/font/caps_type) | Gets and sets the text caps type. |
| [strike_type](/cells/python-net/aspose.cells/font/strike_type) | Gets the strike type of the text. |
| [is_strikeout](/cells/python-net/aspose.cells/font/is_strikeout) | Gets or sets a value indicating whether the font is single strikeout. |
| [script_offset](/cells/python-net/aspose.cells/font/script_offset) | Gets and sets the script offset,in unit of percentage |
| [is_superscript](/cells/python-net/aspose.cells/font/is_superscript) | Gets or sets a value indicating whether the font is super script. |
| [is_subscript](/cells/python-net/aspose.cells/font/is_subscript) | Gets or sets a value indicating whether the font is subscript. |
| [underline](/cells/python-net/aspose.cells/font/underline) | Gets or sets the font underline type. |
| [name](/cells/python-net/aspose.cells/font/name) | Gets  or sets the name of the [`Font`](/cells/python-net/aspose.cells/font). |
| [double_size](/cells/python-net/aspose.cells/font/double_size) | Gets and sets the double size of the font. |
| [size](/cells/python-net/aspose.cells/font/size) | Gets or sets the size of the font. |
| [theme_color](/cells/python-net/aspose.cells/font/theme_color) | Gets and sets the theme color. |
| [color](/cells/python-net/aspose.cells/font/color) | Gets or sets the Color of the font. |
| [argb_color](/cells/python-net/aspose.cells/font/argb_color) | Gets and sets the color with a 32-bit ARGB value. |
| [is_normalize_heights](/cells/python-net/aspose.cells/font/is_normalize_heights) | Indicates whether the normalization of height that is to be applied to the text run. |
| [scheme_type](/cells/python-net/aspose.cells/font/scheme_type) | Gets and sets the scheme type of the font. |
### Methods
| Method | Description |
| :- | :- |
| [`equals(self, font)`](/cells/python-net/aspose.cells/font/equals/#aspose.cells.font) | Checks if two fonts are equals. |
### Example
```python
from aspose.cells import Workbook
from aspose.pydrawing import Color
# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[0]
# Accessing the "A1" cell from the worksheet
cell = worksheet.cells.get("A1")
# Adding some value to the "A1" cell
cell.put_value("Hello Aspose!")
font = cell.get_style().font
# Setting the font name to "Times New Roman"
font.name = "Times New Roman"
# Setting font size to 14
font.size = 14
# setting font color as Red
font.color = Color.red
# Saving the Excel file
workbook.save(r"dest.xls")
```
### See Also
* module [`aspose.cells`](..)
* class [`Font`](/cells/python-net/aspose.cells/font)
