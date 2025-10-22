##ShapeTextAlignment class
## ShapeTextAlignment class
Represents the setting of shape's text alignment;
The ShapeTextAlignment type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [is_text_wrapped](/cells/python-net/aspose.cells.drawing.texts/shapetextalignment/is_text_wrapped) | Gets or sets the text wrapped type of the shape which contains text. |
| [rotate_text_with_shape](/cells/python-net/aspose.cells.drawing.texts/shapetextalignment/rotate_text_with_shape) | Indicates whether rotating text with shape. |
| [text_vertical_overflow](/cells/python-net/aspose.cells.drawing.texts/shapetextalignment/text_vertical_overflow) | Gets and sets the text vertical overflow type of the text box. |
| [text_horizontal_overflow](/cells/python-net/aspose.cells.drawing.texts/shapetextalignment/text_horizontal_overflow) | Gets and sets the text horizontal overflow type of the text box. |
| [rotation_angle](/cells/python-net/aspose.cells.drawing.texts/shapetextalignment/rotation_angle) | Gets and sets the rotation of the shape. |
| [text_vertical_type](/cells/python-net/aspose.cells.drawing.texts/shapetextalignment/text_vertical_type) | Gets and sets the text direction. |
| [is_locked_text](/cells/python-net/aspose.cells.drawing.texts/shapetextalignment/is_locked_text) | Indicates whether the shape is locked when worksheet is protected. |
| [auto_size](/cells/python-net/aspose.cells.drawing.texts/shapetextalignment/auto_size) | Indicates if size of shape is adjusted automatically according to its content. |
| [text_shape_type](/cells/python-net/aspose.cells.drawing.texts/shapetextalignment/text_shape_type) | Gets and set the transform type of text. |
| [top_margin_pt](/cells/python-net/aspose.cells.drawing.texts/shapetextalignment/top_margin_pt) | Returns the top margin in unit of Points |
| [bottom_margin_pt](/cells/python-net/aspose.cells.drawing.texts/shapetextalignment/bottom_margin_pt) | Returns the bottom margin in unit of Points |
| [left_margin_pt](/cells/python-net/aspose.cells.drawing.texts/shapetextalignment/left_margin_pt) | Returns the left margin in unit of Points |
| [right_margin_pt](/cells/python-net/aspose.cells.drawing.texts/shapetextalignment/right_margin_pt) | Returns the right margin in unit of Points |
| [is_auto_margin](/cells/python-net/aspose.cells.drawing.texts/shapetextalignment/is_auto_margin) | Indicates whether the margin of the text frame is automatic. |
| [number_of_columns](/cells/python-net/aspose.cells.drawing.texts/shapetextalignment/number_of_columns) | Gets and sets the number of columns of text in the bounding rectangle. |
### Example
```python
from aspose.cells import Workbook
# Instantiating a Workbook object
workbook = Workbook()
shape = workbook.worksheets[0].shapes.add_rectangle(1, 0, 1, 0, 50, 100)
shapeTextAlignment = shape.text_body.text_alignment
```
### See Also
* module [`aspose.cells.drawing.texts`](..)
