##FontSetting class
## FontSetting class
Represents a range of characters within the cell text.
The FontSetting type exposes the following members:
### Constructors
| Constructor | Description |
| :- | :- |
| [`__init__(self, start_index, length, sheets)`](/cells/python-net/aspose.cells/fontsetting/__init__/#int-int-aspose.cells.worksheetcollection) |  |
### Properties
| Property | Description |
| :- | :- |
| [type](/cells/python-net/aspose.cells/fontsetting/type) | Gets the type of text node. |
| [start_index](/cells/python-net/aspose.cells/fontsetting/start_index) | Gets the start index of the characters. |
| [length](/cells/python-net/aspose.cells/fontsetting/length) | Gets the length of the characters. |
| [font](/cells/python-net/aspose.cells/fontsetting/font) | Returns the font of this object. |
| [text_options](/cells/python-net/aspose.cells/fontsetting/text_options) | Returns the text options. |
### Methods
| Method | Description |
| :- | :- |
| [`set_word_art_style(self, style)`](/cells/python-net/aspose.cells/fontsetting/set_word_art_style/#aspose.cells.drawing.presetwordartstyle) | Sets the preset WordArt style. |
### Example
```python
from aspose.cells import Workbook
from aspose.pydrawing import Color
# Instantiating a Workbook object
workbook = Workbook()
# Adding a new worksheet to the Excel object
workbook.worksheets.add()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[0]
# Accessing the "A1" cell from the worksheet
cell = worksheet.cells.get("A1")
# Adding some value to the "A1" cell
cell.put_value("Visit Aspose!")
# getting charactor
charactor = cell.characters(6, 7)
# Setting the font of selected characters to bold
charactor.font.is_bold = True
# Setting the font color of selected characters to blue
charactor.font.color = Color.blue
# Saving the Excel file
workbook.save("book1.xls")
```
### See Also
* module [`aspose.cells`](..)
