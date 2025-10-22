##default_style property
## default_style property
Gets or sets the default [`Style`](/cells/python-net/aspose.cells/style) object of the workbook.
### Remarks
The DefaultStyle property is useful to implement a Style for the whole Workbook.
### Example
The following code creates and instantiates a new Workbook and sets a default [`Style`](/cells/python-net/aspose.cells/style) to it.
```python
from aspose.cells import Workbook
workbook = Workbook()
defaultStyle = workbook.default_style
defaultStyle.font.name = "Tahoma"
workbook.default_style = defaultStyle
```
### Definition:
```python
@property
def default_style(self):
...
@default_style.setter
def default_style(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`Style`](/cells/python-net/aspose.cells/style)
* class [`Workbook`](/cells/python-net/aspose.cells/workbook)
