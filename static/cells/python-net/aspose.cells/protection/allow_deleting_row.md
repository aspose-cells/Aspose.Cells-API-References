##allow_deleting_row property
## allow_deleting_row property
Represents if the deletion of rows is allowed on a protected worksheet.
### Remarks
The rows containing the cells to be deleted must be unlocked when the sheet is protected,
and "Select unlocked cells" option must be enabled.
### Definition:
```python
@property
def allow_deleting_row(self):
...
@allow_deleting_row.setter
def allow_deleting_row(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`Protection`](/cells/python-net/aspose.cells/protection)
