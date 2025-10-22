##BorderCollection class
## BorderCollection class
Encapsulates a collection of [`Border`](/cells/python-net/aspose.cells/border) objects.
The BorderCollection type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [diagonal_color](/cells/python-net/aspose.cells/bordercollection/diagonal_color) | Gets or sets the Color of Diagonal lines. |
| [diagonal_style](/cells/python-net/aspose.cells/bordercollection/diagonal_style) | Gets or sets the style of Diagonal lines. |
### Methods
| Method | Description |
| :- | :- |
| [`get(self, border_type)`](/cells/python-net/aspose.cells/bordercollection/get/#aspose.cells.bordertype) | Add API for Python Via .Net.since this[BorderType borderType] is unsupported |
| [`set_color(self, color)`](/cells/python-net/aspose.cells/bordercollection/set_color/#aspose.pydrawing.color) | Sets the Color of all borders in the collection. |
| [`set_style(self, style)`](/cells/python-net/aspose.cells/bordercollection/set_style/#aspose.cells.cellbordertype) | Sets the style of all borders of the collection. |
### Example
```python
from aspose.cells import BorderType, CellBorderType, Workbook
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
style = cell.get_style()
# Setting the line style of the top border
style.borders.get(BorderType.TOP_BORDER).line_style = CellBorderType.THICK
# Setting the color of the top border
style.borders.get(BorderType.TOP_BORDER).color = Color.black
# Setting the line style of the bottom border
style.borders.get(BorderType.BOTTOM_BORDER).line_style = CellBorderType.THICK
# Setting the color of the bottom border
style.borders.get(BorderType.BOTTOM_BORDER).color = Color.black
# Setting the line style of the left border
style.borders.get(BorderType.LEFT_BORDER).line_style = CellBorderType.THICK
# Setting the color of the left border
style.borders.get(BorderType.LEFT_BORDER).color = Color.black
# Setting the line style of the right border
style.borders.get(BorderType.RIGHT_BORDER).line_style = CellBorderType.THICK
# Setting the color of the right border
style.borders.get(BorderType.RIGHT_BORDER).color = Color.black
cell.set_style(style)
# Saving the Excel file
workbook.save("book1.xls")
```
### See Also
* module [`aspose.cells`](..)
* class [`Border`](/cells/python-net/aspose.cells/border)
