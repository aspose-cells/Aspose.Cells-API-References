##html_text property
## html_text property
Gets and sets the html string which contains data and some formats in this textbox.
### Example
```python
html = shape.html_text
if html == null  or html == "":
shape.html_text = "<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>"
```
### Definition:
```python
@property
def html_text(self):
...
@html_text.setter
def html_text(self, value):
...
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`SmartArtShape`](/cells/python-net/aspose.cells.drawing/smartartshape)
