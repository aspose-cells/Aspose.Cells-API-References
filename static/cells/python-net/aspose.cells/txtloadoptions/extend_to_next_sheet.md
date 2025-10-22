##extend_to_next_sheet property
## extend_to_next_sheet property
Whether extends data to next sheet when the rows or columns of data exceed limit.
Default is false.
### Remarks
If this property is true, extra data will be put into next sheet behind current one
(if current sheet is the last one, new sheet will be appended to current workbook).
If this property is false, the data exceeding limit will be ignored.
### Definition:
```python
@property
def extend_to_next_sheet(self):
...
@extend_to_next_sheet.setter
def extend_to_next_sheet(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`TxtLoadOptions`](/cells/python-net/aspose.cells/txtloadoptions)
