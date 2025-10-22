##html_note property
## html_note property
Gets and sets the html string which contains data and some formats in this comment.
### Remarks
If this is a threaded comment, the note could not be changed, otherwise MS Excel could not process it as a threaded comment.
### Example
```python
comment1.html_note = "<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>"
```
### Definition:
```python
@property
def html_note(self):
...
@html_note.setter
def html_note(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`Comment`](/cells/python-net/aspose.cells/comment)
