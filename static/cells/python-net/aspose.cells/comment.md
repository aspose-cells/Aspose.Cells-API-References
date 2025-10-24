##Comment class
## Comment class
Encapsulates the object that represents a cell comment.
The Comment type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [author](/cells/python-net/aspose.cells/comment/author) | Gets and sets Name of the original comment author |
| [comment_shape](/cells/python-net/aspose.cells/comment/comment_shape) | Get a Shape object that represents the shape attached to the specified comment. |
| [row](/cells/python-net/aspose.cells/comment/row) | Gets the row index of the comment. |
| [column](/cells/python-net/aspose.cells/comment/column) | Gets the column index of the comment. |
| [is_threaded_comment](/cells/python-net/aspose.cells/comment/is_threaded_comment) | Indicates whether this comment is a threaded comment. |
| [threaded_comments](/cells/python-net/aspose.cells/comment/threaded_comments) | Gets the list of threaded comments; |
| [note](/cells/python-net/aspose.cells/comment/note) | Represents the content of comment. |
| [html_note](/cells/python-net/aspose.cells/comment/html_note) | Gets and sets the html string which contains data and some formats in this comment. |
| [font](/cells/python-net/aspose.cells/comment/font) | Gets the font of comment. |
| [is_visible](/cells/python-net/aspose.cells/comment/is_visible) | Represents if the comment is visible or not. |
| [text_orientation_type](/cells/python-net/aspose.cells/comment/text_orientation_type) | Gets and sets the text orientation type of the comment. |
| [text_horizontal_alignment](/cells/python-net/aspose.cells/comment/text_horizontal_alignment) | Gets and sets the text horizontal alignment type of the comment. |
| [text_vertical_alignment](/cells/python-net/aspose.cells/comment/text_vertical_alignment) | Gets and sets the text vertical alignment type of the comment. |
| [auto_size](/cells/python-net/aspose.cells/comment/auto_size) | Indicates if size of comment is adjusted automatically according to its content.
| [height_cm](/cells/python-net/aspose.cells/comment/height_cm) | Represents the height of the comment, in unit of centimeters. |
| [width_cm](/cells/python-net/aspose.cells/comment/width_cm) | Represents the width of the comment, in unit of centimeters. |
| [width](/cells/python-net/aspose.cells/comment/width) | Represents the width of the comment, in unit of pixels. |
| [height](/cells/python-net/aspose.cells/comment/height) | Represents the Height of the comment, in unit of pixels. |
| [width_inch](/cells/python-net/aspose.cells/comment/width_inch) | Represents the width of the comment, in unit of inches. |
| [height_inch](/cells/python-net/aspose.cells/comment/height_inch) | Represents the height of the comment, in unit of inches. |
### Methods
| Method | Description |
| :- | :- |
| [`format_characters(self, start_index, length, font, flag)`](/cells/python-net/aspose.cells/comment/format_characters/#int-int-aspose.cells.font-aspose.cells.styleflag) | Format some characters with the font setting. |
| [`characters(self, start_index, length)`](/cells/python-net/aspose.cells/comment/characters/#int-int) | Returns a Characters object that represents a range of characters within the comment text. |
| [`get_characters(self)`](/cells/python-net/aspose.cells/comment/get_characters/#) | Returns all Characters objects
| [`get_rich_formattings(self)`](/cells/python-net/aspose.cells/comment/get_rich_formattings/#) | Returns all Characters objects
### Example
```python
from aspose.cells import Workbook
workbook = Workbook()
comments = workbook.worksheets[0].comments
# Add comment to cell A1
commentIndex1 = comments.add(0, 0)
comment1 = comments[commentIndex1]
comment1.note = "First note."
comment1.font.name = "Times New Roman"
# Add comment to cell B2
comments.add("B2")
comment2 = comments.get("B2")
comment2.note = "Second note."
# do your business
# Save the excel file.
workbook.save("exmaple.xlsx")
```
### See Also
* module [`aspose.cells`](..)
