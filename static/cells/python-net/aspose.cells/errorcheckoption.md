##ErrorCheckOption class
## ErrorCheckOption class
Error check setting applied on certain ranges.
The ErrorCheckOption type exposes the following members:
### Methods
| Method | Description |
| :- | :- |
| [`is_error_check(self, error_check_type)`](/cells/python-net/aspose.cells/errorcheckoption/is_error_check/#aspose.cells.errorchecktype) | Checks whether given error type will be checked. |
| [`set_error_check(self, error_check_type, is_check)`](/cells/python-net/aspose.cells/errorcheckoption/set_error_check/#aspose.cells.errorchecktype-bool) | Sets whether given error type will be checked. |
| [`get_count_of_range(self)`](/cells/python-net/aspose.cells/errorcheckoption/get_count_of_range/#) | Gets the count of ranges that influenced by this setting. |
| [`add_range(self, ca)`](/cells/python-net/aspose.cells/errorcheckoption/add_range/#aspose.cells.cellarea) | Adds one influenced range by this setting. |
| [`get_range(self, index)`](/cells/python-net/aspose.cells/errorcheckoption/get_range/#int) | Gets the influenced range of this setting by given index. |
| [`remove_range(self, index)`](/cells/python-net/aspose.cells/errorcheckoption/remove_range/#int) | Removes one range by given index. |
### Example
```python
from aspose.cells import CellArea, ErrorCheckType, Workbook
workbook = Workbook()
opts = workbook.worksheets[0].error_check_options
optionIdx = opts.add()
opt = opts[optionIdx]
opt.set_error_check(ErrorCheckType.INCONSIST_FORMULA, False)
opt.set_error_check(ErrorCheckType.INCONSIST_RANGE, False)
opt.set_error_check(ErrorCheckType.TEXT_DATE, False)
opt.set_error_check(ErrorCheckType.TEXT_NUMBER, False)
opt.set_error_check(ErrorCheckType.VALIDATION, False)
opt.add_range(CellArea.create_cell_area("A1", "B10"))
workbook.save(r"Book1.xlsx")
```
### See Also
* module [`aspose.cells`](..)
