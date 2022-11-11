---
title: WorkbookDesigner
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 1590
url: /cells/python-net/aspose.cells/workbookdesigner/
---

## WorkbookDesigner class

Encapsulates the object that represents a designer spreadsheet.

The WorkbookDesigner type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|WorkbookDesigner()|Initializes a new instance of the [WorkbookDesigner](/cells/python-net/aspose.cells/workbookdesigner/) class.|
|WorkbookDesigner(workbook)|Initializes a new instance of the WorkbookDesigner class|
## Properties
| Name | Description |
| :- | :- |
|workbook|Gets and sets the [workbook](/cells/python-net/aspose.cells/workbookdesigner/) object.|
|repeat_formulas_with_subtotal|Indicates whether repeating formulas with subtotal row.|
|update_empty_string_as_null|If TRUE, Null will be inserted if the value is "";|
|update_reference|Indicates if references in other worksheets will be updated.|
|calculate_formula|Indicates whether formulas should be calculated.|
|call_back|Gets and sets callback interface of processing smartmarker.|
|line_by_line|Indicates whether processing the smart marker line by line.|
## Methods
| Name | Description |
| :- | :- |
|set_data_source(data_source, cells_data_table)|Sets data source of a [ICellsDataTable](/cells/python-net/aspose.cells/icellsdatatable/) object.|
|set_data_source(variable, data)|Sets data binding to a variable.|
|process()|Processes the smart markers and populates the data source values.|
|process(is_preserved)|Processes the smart markers and populates the data source values.|
|process(sheet_index, is_preserved)|Processes the smart markers and populates the data source values.|
|clear_data_source()|Clears all data sources.|
|get_smart_markers()|Returns a collection of smart markers in a spreadsheet.|

### See Also

* namespace [aspose.cells](/cells/python-net/aspose.cells/)
* assembly [Aspose.Cells](/cells/python-net/)

