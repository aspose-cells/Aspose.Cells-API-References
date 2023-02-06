---
title: WorkbookDesigner class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 1600
url: /python-net/aspose.cells/workbookdesigner/
is_root: false
---

## WorkbookDesigner class

Encapsulates the object that represents a designer spreadsheet.



The WorkbookDesigner type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [WorkbookDesigner()](/cells/python-net/aspose.cells/workbookdesigner/__init__/#) | Initializes a new instance of the [WorkbookDesigner](/cells/python-net/aspose.cells/workbookdesigner) class. |
| [WorkbookDesigner(workbook)](/cells/python-net/aspose.cells/workbookdesigner/__init__/#Workbook) | Initializes a new instance of the [WorkbookDesigner](/cells/python-net/aspose.cells/workbookdesigner) class. |


### Properties
| Property | Description |
| :- | :- |
| [workbook](/cells/python-net/aspose.cells/workbookdesigner/workbook) | Gets and sets the [WorkbookDesigner.workbook](/cells/python-net/aspose.cells/workbookdesigner#workbook) object. |
| [repeat_formulas_with_subtotal](/cells/python-net/aspose.cells/workbookdesigner/repeat_formulas_with_subtotal) | Indicates whether repeating formulas with subtotal row. |
| [update_empty_string_as_null](/cells/python-net/aspose.cells/workbookdesigner/update_empty_string_as_null) | If TRUE, Null will be inserted if the value is ""; |
| [update_reference](/cells/python-net/aspose.cells/workbookdesigner/update_reference) | Indicates if references in other worksheets will be updated. |
| [calculate_formula](/cells/python-net/aspose.cells/workbookdesigner/calculate_formula) | Indicates whether formulas should be calculated. |
| [call_back](/cells/python-net/aspose.cells/workbookdesigner/call_back) | Gets and sets callback interface of processing smartmarker. |
| [line_by_line](/cells/python-net/aspose.cells/workbookdesigner/line_by_line) | Indicates whether processing the smart marker line by line. |


### Methods
| Method | Description |
| :- | :- |
| [set_data_source(data_source, cells_data_table)](/cells/python-net/aspose.cells/workbookdesigner/set_data_source/#str-ICellsDataTable) | Sets data source of a [ICellsDataTable](/cells/python-net/aspose.cells/icellsdatatable) object. |
| [set_data_source(variable, data)](/cells/python-net/aspose.cells/workbookdesigner/set_data_source/#str-any) | Sets data binding to a variable. |
| [process()](/cells/python-net/aspose.cells/workbookdesigner/process/#) | Processes the smart markers and populates the data source values. |
| [process(is_preserved)](/cells/python-net/aspose.cells/workbookdesigner/process/#bool) | Processes the smart markers and populates the data source values. |
| [process(sheet_index, is_preserved)](/cells/python-net/aspose.cells/workbookdesigner/process/#int-bool) | Processes the smart markers and populates the data source values. |
| [clear_data_source()](/cells/python-net/aspose.cells/workbookdesigner/clear_data_source/#) | Clears all data sources. |
| [get_smart_markers()](/cells/python-net/aspose.cells/workbookdesigner/get_smart_markers/#) | Returns a collection of smart markers in a spreadsheet. |



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
* module [aspose.cells](..)
* class [ICellsDataTable](/cells/python-net/aspose.cells/icellsdatatable)
* class [WorkbookDesigner](/cells/python-net/aspose.cells/workbookdesigner)
