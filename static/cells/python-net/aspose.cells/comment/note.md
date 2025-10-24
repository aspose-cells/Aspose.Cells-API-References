##note property
## note property
Represents the content of comment.
### Remarks
If this is a threaded comment, the note could not be changed, otherwise MS Excel could not process it as a threaded comment.
### Example
```python
comment1.note = "First note."
```
### Definition:
```python
@property
def note(self):
...
@note.setter
def note(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`Comment`](/cells/python-net/aspose.cells/comment)
