##TextBoxOptions class
## TextBoxOptions class
Represents the text options of the shape
The TextBoxOptions type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [shape_text_vertical_alignment](/cells/python-net/aspose.cells.drawing.texts/textboxoptions/shape_text_vertical_alignment) | It corresponds to "Format Shape - Text Options - Text Box - Vertical Alignment" in Excel. |
| [resize_to_fit_text](/cells/python-net/aspose.cells.drawing.texts/textboxoptions/resize_to_fit_text) | Indicates whether to resize the shape to fit the text |
| [shape_text_direction](/cells/python-net/aspose.cells.drawing.texts/textboxoptions/shape_text_direction) | Gets or sets the text display direction within a given text body.
| [left_margin_pt](/cells/python-net/aspose.cells.drawing.texts/textboxoptions/left_margin_pt) | Gets and sets the left margin in unit of Points. |
| [right_margin_pt](/cells/python-net/aspose.cells.drawing.texts/textboxoptions/right_margin_pt) | Gets and sets the right margin in unit of Points. |
| [top_margin_pt](/cells/python-net/aspose.cells.drawing.texts/textboxoptions/top_margin_pt) | Gets and sets the top margin in unit of Points. |
| [bottom_margin_pt](/cells/python-net/aspose.cells.drawing.texts/textboxoptions/bottom_margin_pt) | Returns the bottom margin in unit of Points |
| [allow_text_to_overflow](/cells/python-net/aspose.cells.drawing.texts/textboxoptions/allow_text_to_overflow) | Whether allow text to overflow shape. |
| [wrap_text_in_shape](/cells/python-net/aspose.cells.drawing.texts/textboxoptions/wrap_text_in_shape) | Specifies text wrapping within a shape.
### Example
```python
from aspose.cells import Workbook
# Instantiating a Workbook object
workbook = Workbook()
index = workbook.worksheets[0].text_boxes.add(0, 0, 350, 350)
shape = workbook.worksheets[0].text_boxes[index]
shape.text = "This is test."
# do your business
# Save the excel file.
workbook.save("exmaple.xlsx")
```
### See Also
* module [`aspose.cells.drawing.texts`](..)
