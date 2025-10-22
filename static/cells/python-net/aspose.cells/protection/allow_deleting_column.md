##allow_deleting_column property
## allow_deleting_column property
Represents if the deletion of columns is allowed on a protected worksheet.
### Remarks
The columns containing the cells to be deleted must be unlocked when the sheet is protected,
and "Select unlocked cells" option must be enabled.
### Definition:
```python
@property
def allow_deleting_column(self):
...
@allow_deleting_column.setter
def allow_deleting_column(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`Protection`](/cells/python-net/aspose.cells/protection)
