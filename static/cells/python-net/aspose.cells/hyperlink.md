##Hyperlink class
## Hyperlink class
Encapsulates the object that represents a hyperlink.
The Hyperlink type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [address](/cells/python-net/aspose.cells/hyperlink/address) | Represents the address of a hyperlink. |
| [text_to_display](/cells/python-net/aspose.cells/hyperlink/text_to_display) | Represents the text to be displayed for the specified hyperlink. The default value is the address of the hyperlink. |
| [area](/cells/python-net/aspose.cells/hyperlink/area) | Gets the range of hyperlink. |
| [screen_tip](/cells/python-net/aspose.cells/hyperlink/screen_tip) | Returns or sets the ScreenTip text for the specified hyperlink. |
| [link_type](/cells/python-net/aspose.cells/hyperlink/link_type) | Gets the link type. |
### Methods
| Method | Description |
| :- | :- |
| [`delete(self)`](/cells/python-net/aspose.cells/hyperlink/delete/#) | Deletes this hyperlink |
### Example
```python
from aspose.cells import Workbook
# Instantiating a Workbook object
workbook = Workbook()
# Adding a new worksheet to the Workbook object
workbook.worksheets.add()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[0]
# Adding a hyperlink to a URL at "A1" cell
index = worksheet.hyperlinks.add("A1", 1, 1, "http://www.aspose.com")
# Getting a Hyperlink by index.
hyperlink = worksheet.hyperlinks[index]
# Setting display text of this hyperlink.
hyperlink.text_to_display = "Aspose"
# Saving the Excel file
workbook.save("book1.xls")
```
### See Also
* module [`aspose.cells`](..)
