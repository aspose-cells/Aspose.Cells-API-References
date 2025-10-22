##is_height_matched property
## is_height_matched property
Indicates whether the row height matches current default font setting of the workbook.
True of this property also denotes the row height is "automatic" without custom height value set by user.
### Remarks
When this property is true, if the content in this row changes,
generally the row height needs to be re-calculated(such as by [`Worksheet.auto_fit_rows`](/cells/python-net/aspose.cells/worksheet/auto_fit_rows))
to get the same result with what is shown in ms excel when you opening the workbook in it.
### Definition:
```python
@property
def is_height_matched(self):
...
@is_height_matched.setter
def is_height_matched(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`Row`](/cells/python-net/aspose.cells/row)
