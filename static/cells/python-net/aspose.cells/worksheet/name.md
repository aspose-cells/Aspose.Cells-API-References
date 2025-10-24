##name property
## name property
Gets or sets the name of the worksheet.
### Remarks
The max length of sheet name is 31. And you cannot assign same name(case insensitive) to two worksheets.
For example, you cannot set "SheetName1" to the first worksheet and set "SHEETNAME1" to the second worksheet.
### Definition:
```python
@property
def name(self):
...
@name.setter
def name(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`Worksheet`](/cells/python-net/aspose.cells/worksheet)
