##GridWorkbookSettings class
## GridWorkbookSettings class
Represents the settings of the workbook.
The GridWorkbookSettings type exposes the following members:
### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/cells/python-net/aspose.cellsgridjs/gridworkbooksettings/__init__/#) | Constructs a new instance of GridWorkbookSettings |
### Properties
| Property | Description |
| :- | :- |
| [max_iteration](/cells/python-net/aspose.cellsgridjs/gridworkbooksettings/max_iteration) | Returns or sets the maximum number of iterations to resolve a circular reference,the default value is 100. |
| [iteration](/cells/python-net/aspose.cellsgridjs/gridworkbooksettings/iteration) | Indicates whether use iteration to resolve circular references. |
| [force_full_calculate](/cells/python-net/aspose.cellsgridjs/gridworkbooksettings/force_full_calculate) | Indicates whether fully calculates every time when a calculation is triggered. |
| [create_calc_chain](/cells/python-net/aspose.cellsgridjs/gridworkbooksettings/create_calc_chain) | Indicates whether create calculated formulas chain. Default is false. |
| [re_calculate_on_open](/cells/python-net/aspose.cellsgridjs/gridworkbooksettings/re_calculate_on_open) | Indicates whether re-calculate all formulas on opening file. |
| [precision_as_displayed](/cells/python-net/aspose.cellsgridjs/gridworkbooksettings/precision_as_displayed) | True if calculations in this workbook will be done using only the precision of   the numbers as they're displayed |
| [date1904](/cells/python-net/aspose.cellsgridjs/gridworkbooksettings/date1904) | Gets or sets a value which represents if the workbook uses the 1904 date system. |
| [enable_macros](/cells/python-net/aspose.cellsgridjs/gridworkbooksettings/enable_macros) | Enable macros; Now it only works when copying a worksheet to other worksheet in a workbook. |
| [check_custom_number_format](/cells/python-net/aspose.cellsgridjs/gridworkbooksettings/check_custom_number_format) | Indicates whether checking custom number format when setting Style.Custom. |
| [author](/cells/python-net/aspose.cellsgridjs/gridworkbooksettings/author) | Gets/sets the author of the file. |
### Example
```python
from aspose.cellsgridjs import GridJsWorkbook, GridWorkbookSettings
g = GridJsWorkbook()
gsettings = GridWorkbookSettings()
g.settings = gsettings
```
### See Also
* module [`aspose.cellsgridjs`](..)
