---
title: Validation
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 1530
url: /python-net/aspose.cells/validation/
---

## Validation class

Represents data validation.settings.

The Validation type exposes the following members:
## Properties
| Name | Description |
| :- | :- |
|operator|Represents the operator for the data validation.|
|alert_style|Represents the validation alert style.|
|type|Represents the data validation type.|
|input_message|Represents the data validation input message.|
|input_title|Represents the title of the data-validation input dialog box.|
|error_message|Represents the data validation error message.|
|error_title|Represents the title of the data-validation error dialog box.|
|show_input|Indicates whether the data validation input message will be displayed whenever the user selects a cell in the data validation range.|
|show_error|Indicates whether the data validation error message will be displayed whenever the user enters invalid data.|
|ignore_blank|Indicates whether blank values are permitted by the range data validation.|
|formula1|Represents the value or expression associated with the data validation.|
|formula2|Represents the value or expression associated with the data validation.|
|value1|Represents the first value associated with the data validation.|
|value2|Represents the second value associated with the data validation.|
|in_cell_drop_down|Indicates whether data validation displays a drop-down list that contains acceptable values.|
|areas|Gets all [CellArea](/python-net/aspose.cells/cellarea/) which contain the data validation settings.|
## Methods
| Name | Description |
| :- | :- |
|get_formula1(is_r1c1, is_local)|Gets the value or expression associated with this validation.|
|get_formula1(is_r1c1, is_local, row, column)|Gets the value or expression associated with this validation for specific cell.|
|get_formula2(is_r1c1, is_local)|Gets the value or expression associated with this validation.|
|get_formula2(is_r1c1, is_local, row, column)|Gets the value or expression associated with this validation for specific cell.|
|add_area(cell_area)|Applies the validation to the area.|
|add_area(cell_area, check_intersection, check_edge)|Applies the validation to the area.|
|set_formula1(formula, is_r1c1, is_local)|Sets the value or expression associated with this validation.|
|set_formula2(formula, is_r1c1, is_local)|Sets the value or expression associated with this validation.|
|get_list_value(row, column)|Get the value for list of the validation for the specified cell.|
|add_areas(areas, check_intersection, check_edge)|Applies the validation to given areas.|
|remove_area(cell_area)|Remove the validation settings in the range.|
|remove_areas(areas)|Removes this validation from given areas.|
|remove_a_cell(row, column)|Remove the validation settings in the cell.|
|copy(source, copy_option)|Copy validation.|

### See Also

* namespace [aspose.cells](/python-net/aspose.cells/)
* assembly [Aspose.Cells](/python-net/)

