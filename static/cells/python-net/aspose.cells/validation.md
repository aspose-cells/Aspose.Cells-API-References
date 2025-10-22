##Validation class
## Validation class
Represents data validation.settings.
The Validation type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [operator](/cells/python-net/aspose.cells/validation/operator) | Represents the operator for the data validation. |
| [alert_style](/cells/python-net/aspose.cells/validation/alert_style) | Represents the validation alert style. |
| [type](/cells/python-net/aspose.cells/validation/type) | Represents the data validation type. |
| [input_message](/cells/python-net/aspose.cells/validation/input_message) | Represents the data validation input message. |
| [input_title](/cells/python-net/aspose.cells/validation/input_title) | Represents the title of the data-validation input dialog box. |
| [error_message](/cells/python-net/aspose.cells/validation/error_message) | Represents the data validation error message. |
| [error_title](/cells/python-net/aspose.cells/validation/error_title) | Represents the title of the data-validation error dialog box. |
| [show_input](/cells/python-net/aspose.cells/validation/show_input) | Indicates whether the data validation input message will be displayed whenever the user selects a cell in the data validation range. |
| [show_error](/cells/python-net/aspose.cells/validation/show_error) | Indicates whether the data validation error message will be displayed whenever the user enters invalid data. |
| [ignore_blank](/cells/python-net/aspose.cells/validation/ignore_blank) | Indicates whether blank values are permitted by the range data validation. |
| [formula1](/cells/python-net/aspose.cells/validation/formula1) | Represents the value or expression associated with the data validation. |
| [formula2](/cells/python-net/aspose.cells/validation/formula2) | Represents the value or expression associated with the data validation. |
| [value1](/cells/python-net/aspose.cells/validation/value1) | Represents the first value associated with the data validation. |
| [value2](/cells/python-net/aspose.cells/validation/value2) | Represents the second value associated with the data validation. |
| [in_cell_drop_down](/cells/python-net/aspose.cells/validation/in_cell_drop_down) | Indicates whether data validation displays a drop-down list that contains acceptable values. |
| [areas](/cells/python-net/aspose.cells/validation/areas) | Gets all [`CellArea`](/cells/python-net/aspose.cells/cellarea) which contain the data validation settings. |
### Methods
| Method | Description |
| :- | :- |
| [`get_formula1(self, is_r1c1, is_local)`](/cells/python-net/aspose.cells/validation/get_formula1/#bool-bool) | Gets the value or expression associated with this validation. |
| [`get_formula1(self, is_r1c1, is_local, row, column)`](/cells/python-net/aspose.cells/validation/get_formula1/#bool-bool-int-int) | Gets the value or expression associated with this validation for specific cell. |
| [`get_formula2(self, is_r1c1, is_local)`](/cells/python-net/aspose.cells/validation/get_formula2/#bool-bool) | Gets the value or expression associated with this validation. |
| [`get_formula2(self, is_r1c1, is_local, row, column)`](/cells/python-net/aspose.cells/validation/get_formula2/#bool-bool-int-int) | Gets the value or expression associated with this validation for specific cell. |
| [`add_area(self, cell_area)`](/cells/python-net/aspose.cells/validation/add_area/#aspose.cells.cellarea) | Applies the validation to the area. |
| [`add_area(self, cell_area, check_intersection, check_edge)`](/cells/python-net/aspose.cells/validation/add_area/#aspose.cells.cellarea-bool-bool) | Applies the validation to the area. |
| [`set_formula1(self, formula, is_r1c1, is_local)`](/cells/python-net/aspose.cells/validation/set_formula1/#system.string-bool-bool) | Sets the value or expression associated with this validation. |
| [`set_formula2(self, formula, is_r1c1, is_local)`](/cells/python-net/aspose.cells/validation/set_formula2/#system.string-bool-bool) | Sets the value or expression associated with this validation. |
| [`get_list_value(self, row, column)`](/cells/python-net/aspose.cells/validation/get_list_value/#int-int) | Get the value for list of the validation for the specified cell. |
| [`get_value(self, row, column, is_value1)`](/cells/python-net/aspose.cells/validation/get_value/#int-int-bool) | Get the value of validation on the specific cell. |
| [`add_areas(self, areas, check_intersection, check_edge)`](/cells/python-net/aspose.cells/validation/add_areas/#list-bool-bool) | Applies the validation to given areas. |
| [`remove_area(self, cell_area)`](/cells/python-net/aspose.cells/validation/remove_area/#aspose.cells.cellarea) | Remove the validation settings in the range. |
| [`remove_areas(self, areas)`](/cells/python-net/aspose.cells/validation/remove_areas/#list) | Removes this validation from given areas. |
| [`remove_a_cell(self, row, column)`](/cells/python-net/aspose.cells/validation/remove_a_cell/#int-int) | Remove the validation settings in the cell. |
| [`copy(self, source, copy_option)`](/cells/python-net/aspose.cells/validation/copy/#aspose.cells.validation-aspose.cells.copyoptions) | Copy validation. |
### Example
```python
from aspose.cells import CellArea, OperatorType, ValidationType, Workbook
workbook = Workbook()
validations = workbook.worksheets[0].validations
area = CellArea.create_cell_area(0, 0, 1, 1)
validation = validations[validations.add(area)]
validation.type = ValidationType.WHOLE_NUMBER
validation.operator = OperatorType.BETWEEN
validation.formula1 = "3"
validation.formula2 = "1234"
```
### See Also
* module [`aspose.cells`](..)
* class [`CellArea`](/cells/python-net/aspose.cells/cellarea)
