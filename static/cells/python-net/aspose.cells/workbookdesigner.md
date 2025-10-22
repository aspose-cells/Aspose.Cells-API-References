##WorkbookDesigner class
## WorkbookDesigner class
Encapsulates the object that represents a designer spreadsheet.
The WorkbookDesigner type exposes the following members:
### Constructors
| Constructor | Description |
| :- | :- |
| [`__init__(self)`](/cells/python-net/aspose.cells/workbookdesigner/__init__/#) | Initializes a new instance of the [`WorkbookDesigner`](/cells/python-net/aspose.cells/workbookdesigner) class. |
| [`__init__(self, workbook)`](/cells/python-net/aspose.cells/workbookdesigner/__init__/#aspose.cells.workbook) | Initializes a new instance of the [`WorkbookDesigner`](/cells/python-net/aspose.cells/workbookdesigner) class. |
### Properties
| Property | Description |
| :- | :- |
| [workbook](/cells/python-net/aspose.cells/workbookdesigner/workbook) | Gets and sets the [`WorkbookDesigner.workbook`](/cells/python-net/aspose.cells/workbookdesigner#workbook) object. |
| [repeat_formulas_with_subtotal](/cells/python-net/aspose.cells/workbookdesigner/repeat_formulas_with_subtotal) | Indicates whether repeating formulas with subtotal row. |
| [update_empty_string_as_null](/cells/python-net/aspose.cells/workbookdesigner/update_empty_string_as_null) | If TRUE, Null will be inserted if the value is ""; |
| [update_reference](/cells/python-net/aspose.cells/workbookdesigner/update_reference) | Indicates if references in other worksheets will be updated. |
| [calculate_formula](/cells/python-net/aspose.cells/workbookdesigner/calculate_formula) | Indicates whether formulas should be calculated. |
| [call_back](/cells/python-net/aspose.cells/workbookdesigner/call_back) | Gets and sets callback interface of processing smartmarker. |
| [line_by_line](/cells/python-net/aspose.cells/workbookdesigner/line_by_line) | Indicates whether processing the smart marker line by line. |
| [contains_variables](/cells/python-net/aspose.cells/workbookdesigner/contains_variables) | Indicates whether the first worksheet contains custom variables. |
| [sort_data_source](/cells/python-net/aspose.cells/workbookdesigner/sort_data_source) | Indicates whether sorting data source. |
### Methods
| Method | Description |
| :- | :- |
| [`set_data_source(self, data_source, cells_data_table)`](/cells/python-net/aspose.cells/workbookdesigner/set_data_source/#system.string-aspose.cells.icellsdatatable) | Sets data source of a [`ICellsDataTable`](/cells/python-net/aspose.cells/icellsdatatable) object. |
| [`set_data_source(self, variable, data)`](/cells/python-net/aspose.cells/workbookdesigner/set_data_source/#system.string-system.object) | Sets data binding to a variable. |
| [`process(self, range, is_preserved)`](/cells/python-net/aspose.cells/workbookdesigner/process/#aspose.cells.range-bool) | Processes the smart markers and populates the data source values. |
| [`process(self)`](/cells/python-net/aspose.cells/workbookdesigner/process/#) | Processes the smart markers and populates the data source values. |
| [`process(self, is_preserved)`](/cells/python-net/aspose.cells/workbookdesigner/process/#bool) | Processes the smart markers and populates the data source values. |
| [`process(self, sheet_index, is_preserved)`](/cells/python-net/aspose.cells/workbookdesigner/process/#int-bool) | Processes the smart markers and populates the data source values. |
| [`clear_data_source(self)`](/cells/python-net/aspose.cells/workbookdesigner/clear_data_source/#) | Clears all data sources. |
| [`set_json_data_source(self, name, json)`](/cells/python-net/aspose.cells/workbookdesigner/set_json_data_source/#system.string-system.string) | Set json string value as data source of smart markers. |
| [`get_smart_markers(self)`](/cells/python-net/aspose.cells/workbookdesigner/get_smart_markers/#) | Returns a collection of smart markers in a spreadsheet. |
### Example
```python
from aspose.cells import Workbook, WorkbookDesigner
# Create WorkbookDesigner object.
wd = WorkbookDesigner()
# Open the template file (which contains smart markers).
wd.workbook = Workbook("SmartMarker_Designer.xls")
# Initialize your data from data source
# DataSet ds = new DataSet();
# ...
# Set the datatable as the data source.
# wd.SetDataSource(dt);
# Process the smart markers to fill the data into the worksheets.
wd.process(True)
# Save the excel file.
wd.workbook.save("outSmartMarker_Designer.xls")
```
### See Also
* module [`aspose.cells`](..)
* class [`ICellsDataTable`](/cells/python-net/aspose.cells/icellsdatatable)
* class [`WorkbookDesigner`](/cells/python-net/aspose.cells/workbookdesigner)
