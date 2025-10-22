##Cell class
## Cell class
Encapsulates the object that represents a single Workbook cell.
The Cell type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [worksheet](/cells/python-net/aspose.cells/cell/worksheet) | Gets the parent worksheet. |
| [date_time_value](/cells/python-net/aspose.cells/cell/date_time_value) | Gets the DateTime value contained in the cell. |
| [row](/cells/python-net/aspose.cells/cell/row) | Gets row number (zero based) of the cell. |
| [column](/cells/python-net/aspose.cells/cell/column) | Gets column number (zero based) of the cell. |
| [is_formula](/cells/python-net/aspose.cells/cell/is_formula) | Represents if the specified cell contains formula. |
| [has_custom_function](/cells/python-net/aspose.cells/cell/has_custom_function) | Checks whether there is custom function(unsupported function) in this cell's formula. |
| [type](/cells/python-net/aspose.cells/cell/type) | Represents cell value type. |
| [name](/cells/python-net/aspose.cells/cell/name) | Gets the name of the cell. |
| [is_error_value](/cells/python-net/aspose.cells/cell/is_error_value) | Checks if the value of this cell is an error. |
| [is_numeric_value](/cells/python-net/aspose.cells/cell/is_numeric_value) | Indicates whether the value of this cell is numeric(int, double and datetime) |
| [string_value](/cells/python-net/aspose.cells/cell/string_value) | Gets the string value contained in the cell. If the type of this cell is string, then return the string value itself.
| [string_value_without_format](/cells/python-net/aspose.cells/cell/string_value_without_format) | Gets cell's value as string without any format. |
| [number_category_type](/cells/python-net/aspose.cells/cell/number_category_type) | Represents the category type of this cell's number formatting. |
| [display_string_value](/cells/python-net/aspose.cells/cell/display_string_value) | Gets the formatted string value of this cell by cell's display style. |
| [int_value](/cells/python-net/aspose.cells/cell/int_value) | Gets the integer value contained in the cell. |
| [double_value](/cells/python-net/aspose.cells/cell/double_value) | Gets the double value contained in the cell. |
| [float_value](/cells/python-net/aspose.cells/cell/float_value) | Gets the float value contained in the cell. |
| [bool_value](/cells/python-net/aspose.cells/cell/bool_value) | Gets the boolean value contained in the cell. |
| [has_custom_style](/cells/python-net/aspose.cells/cell/has_custom_style) | Indicates whether this cell has custom style settings(different from the default one inherited
| [shared_style_index](/cells/python-net/aspose.cells/cell/shared_style_index) | Gets cell's shared style index in the style pool. |
| [formula](/cells/python-net/aspose.cells/cell/formula) | Gets or sets a formula of the [`Cell`](/cells/python-net/aspose.cells/cell). |
| [formula_local](/cells/python-net/aspose.cells/cell/formula_local) | Get the locale formatted formula of the cell. |
| [r1c1_formula](/cells/python-net/aspose.cells/cell/r1c1_formula) | Gets or sets a R1C1 formula of the [`Cell`](/cells/python-net/aspose.cells/cell). |
| [contains_external_link](/cells/python-net/aspose.cells/cell/contains_external_link) | Indicates whether this cell contains an external link.
| [is_array_header](/cells/python-net/aspose.cells/cell/is_array_header) | Indicates the cell's formula is an array formula
| [is_dynamic_array_formula](/cells/python-net/aspose.cells/cell/is_dynamic_array_formula) | Indicates whether the cell's formula is dynamic array formula(true) or legacy array formula(false). |
| [is_array_formula](/cells/python-net/aspose.cells/cell/is_array_formula) | Indicates whether the cell formula is an array formula. |
| [is_in_array](/cells/python-net/aspose.cells/cell/is_in_array) | Indicates whether the cell formula is an array formula. |
| [is_shared_formula](/cells/python-net/aspose.cells/cell/is_shared_formula) | Indicates whether the cell formula is part of shared formula. |
| [is_table_formula](/cells/python-net/aspose.cells/cell/is_table_formula) | Indicates whether this cell is part of table formula. |
| [is_in_table](/cells/python-net/aspose.cells/cell/is_in_table) | Indicates whether this cell is part of table formula. |
| [value](/cells/python-net/aspose.cells/cell/value) | Gets/sets the value contained in this cell. |
| [is_style_set](/cells/python-net/aspose.cells/cell/is_style_set) | Indicates if the cell's style is set. If return false, it means this cell has a default cell format. |
| [is_merged](/cells/python-net/aspose.cells/cell/is_merged) | Checks if a cell is part of a merged range or not. |
| [comment](/cells/python-net/aspose.cells/cell/comment) | Gets the comment of this cell. |
| [html_string](/cells/python-net/aspose.cells/cell/html_string) | Gets and sets the html string which contains data and some formats in this cell. |
| [is_check_box_style](/cells/python-net/aspose.cells/cell/is_check_box_style) | Indicates whether setting this cell as a check box. |
| [embedded_image](/cells/python-net/aspose.cells/cell/embedded_image) | Gets and sets the embeddedn image in the cell. |
### Methods
| Method | Description |
| :- | :- |
| [`put_value(self, bool_value)`](/cells/python-net/aspose.cells/cell/put_value/#bool) | Puts a boolean value into the cell. |
| [`put_value(self, int_value)`](/cells/python-net/aspose.cells/cell/put_value/#int) | Puts an integer value into the cell. |
| [`put_value(self, double_value)`](/cells/python-net/aspose.cells/cell/put_value/#float) | Puts a double value into the cell. |
| [`put_value(self, string_value, is_converted, set_style)`](/cells/python-net/aspose.cells/cell/put_value/#system.string-bool-bool) | Puts a value into the cell, if appropriate the value will be converted to other data type and cell's number format will be reset. |
| [`put_value(self, string_value, is_converted)`](/cells/python-net/aspose.cells/cell/put_value/#system.string-bool) | Puts a string value into the cell and converts the value to other data type if appropriate. |
| [`put_value(self, string_value)`](/cells/python-net/aspose.cells/cell/put_value/#system.string) | Puts a string value into the cell. |
| [`put_value(self, date_time)`](/cells/python-net/aspose.cells/cell/put_value/#system.datetime) | Puts a DateTime value into the cell. |
| [`put_value(self, object_value)`](/cells/python-net/aspose.cells/cell/put_value/#system.object) | Puts an object value into the cell. |
| [`get_display_style(self)`](/cells/python-net/aspose.cells/cell/get_display_style/#) | Gets the display style of this cell. |
| [`get_display_style(self, include_merged_borders)`](/cells/python-net/aspose.cells/cell/get_display_style/#bool) | Gets the display style of this cell. |
| [`get_display_style(self, adjacent_borders)`](/cells/python-net/aspose.cells/cell/get_display_style/#aspose.cells.bordertype) | Gets the display style of this cell. |
| [`get_style(self)`](/cells/python-net/aspose.cells/cell/get_style/#) | Gets the cell style. |
| [`get_style(self, check_borders)`](/cells/python-net/aspose.cells/cell/get_style/#bool) | If checkBorders is true, check whether other cells' borders will effect the style of this cell. |
| [`set_style(self, style)`](/cells/python-net/aspose.cells/cell/set_style/#aspose.cells.style) | Sets the cell style. |
| [`set_style(self, style, explicit_flag)`](/cells/python-net/aspose.cells/cell/set_style/#aspose.cells.style-bool) | Apply the changed property of style to the cell. |
| [`set_style(self, style, flag)`](/cells/python-net/aspose.cells/cell/set_style/#aspose.cells.style-aspose.cells.styleflag) | Apply the cell style based on flags. |
| [`set_formula(self, formula, value)`](/cells/python-net/aspose.cells/cell/set_formula/#system.string-system.object) | Set the formula and the value(calculated result) of the formula. |
| [`set_formula(self, formula, options)`](/cells/python-net/aspose.cells/cell/set_formula/#system.string-aspose.cells.formulaparseoptions) | Set the formula and the value(calculated result) of the formula. |
| [`set_formula(self, formula, is_r1c1, is_local, value)`](/cells/python-net/aspose.cells/cell/set_formula/#system.string-bool-bool-system.object) | Set the formula and the value of the formula. |
| [`set_formula(self, formula, options, value)`](/cells/python-net/aspose.cells/cell/set_formula/#system.string-aspose.cells.formulaparseoptions-system.object) | Set the formula and the value(calculated result) of the formula. |
| [`set_array_formula(self, array_formula, row_number, column_number, is_r1c1, is_local)`](/cells/python-net/aspose.cells/cell/set_array_formula/#system.string-int-int-bool-bool) | Sets an array formula to a range of cells. |
| [`set_array_formula(self, array_formula, row_number, column_number)`](/cells/python-net/aspose.cells/cell/set_array_formula/#system.string-int-int) | Sets an array formula(legacy array formula entered via CTRL+SHIFT+ENTER in ms excel) to a range of cells. |
| [`set_array_formula(self, array_formula, row_number, column_number, options)`](/cells/python-net/aspose.cells/cell/set_array_formula/#system.string-int-int-aspose.cells.formulaparseoptions) | Sets an array formula to a range of cells. |
| [`set_array_formula(self, array_formula, row_number, column_number, options, values)`](/cells/python-net/aspose.cells/cell/set_array_formula/#system.string-int-int-aspose.cells.formulaparseoptions-list) | Sets an array formula to a range of cells. |
| [`set_shared_formula(self, shared_formula, row_number, column_number, is_r1c1, is_local)`](/cells/python-net/aspose.cells/cell/set_shared_formula/#system.string-int-int-bool-bool) | Sets a formula to a range of cells. |
| [`set_shared_formula(self, shared_formula, row_number, column_number)`](/cells/python-net/aspose.cells/cell/set_shared_formula/#system.string-int-int) | Sets shared formulas to a range of cells. |
| [`set_shared_formula(self, shared_formula, row_number, column_number, options)`](/cells/python-net/aspose.cells/cell/set_shared_formula/#system.string-int-int-aspose.cells.formulaparseoptions) | Sets shared formulas to a range of cells. |
| [`set_shared_formula(self, shared_formula, row_number, column_number, options, values)`](/cells/python-net/aspose.cells/cell/set_shared_formula/#system.string-int-int-aspose.cells.formulaparseoptions-list) | Sets shared formulas to a range of cells. |
| [`get_leafs(self)`](/cells/python-net/aspose.cells/cell/get_leafs/#) | Get all cells which reference to this cell directly and need to be updated when this cell is modified. |
| [`get_leafs(self, recursive)`](/cells/python-net/aspose.cells/cell/get_leafs/#bool) | Get all cells which will be updated when this cell is modified. |
| [`set_dynamic_array_formula(self, array_formula, options, calculate_value)`](/cells/python-net/aspose.cells/cell/set_dynamic_array_formula/#system.string-aspose.cells.formulaparseoptions-bool) | Sets dynamic array formula and make the formula spill into neighboring cells if possible. |
| [`set_dynamic_array_formula(self, array_formula, options, values, calculate_range, calculate_value)`](/cells/python-net/aspose.cells/cell/set_dynamic_array_formula/#system.string-aspose.cells.formulaparseoptions-list-bool-bool) | Sets dynamic array formula and make the formula spill into neighboring cells if possible. |
| [`set_dynamic_array_formula(self, array_formula, options, values, calculate_range, calculate_value, copts)`](/cells/python-net/aspose.cells/cell/set_dynamic_array_formula/#system.string-aspose.cells.formulaparseoptions-list-bool-bool-aspose.cells.calculationoptions) | Sets dynamic array formula and make the formula spill into neighboring cells if possible. |
| [`set_table_formula(self, row_number, column_number, row_input_cell, column_input_cell, values)`](/cells/python-net/aspose.cells/cell/set_table_formula/#int-int-system.string-system.string-list) | Create two-variable data table for given range starting from this cell. |
| [`set_table_formula(self, row_number, column_number, input_cell, is_row_input, values)`](/cells/python-net/aspose.cells/cell/set_table_formula/#int-int-system.string-bool-list) | Create one-variable data table for given range starting from this cell. |
| [`set_table_formula(self, row_number, column_number, row_index_of_row_input_cell, column_index_of_row_input_cell, row_index_of_column_input_cell, column_index_of_column_input_cell, values)`](/cells/python-net/aspose.cells/cell/set_table_formula/#int-int-int-int-int-int-list) | Create two-variable data table for given range starting from this cell. |
| [`set_table_formula(self, row_number, column_number, row_index_of_input_cell, column_index_of_input_cell, is_row_input, values)`](/cells/python-net/aspose.cells/cell/set_table_formula/#int-int-int-int-bool-list) | Create one-variable data table for given range starting from this cell. |
| [`get_characters(self)`](/cells/python-net/aspose.cells/cell/get_characters/#) | Returns all Characters objects
| [`get_characters(self, flag)`](/cells/python-net/aspose.cells/cell/get_characters/#bool) | Returns all Characters objects
| [`calculate(self, options)`](/cells/python-net/aspose.cells/cell/calculate/#aspose.cells.calculationoptions) | Calculates the formula of the cell. |
| [`get_string_value(self, format_strategy)`](/cells/python-net/aspose.cells/cell/get_string_value/#aspose.cells.cellvalueformatstrategy) | Gets the string value by specific formatted strategy. |
| [`get_width_of_value(self)`](/cells/python-net/aspose.cells/cell/get_width_of_value/#) | Gets the width of the value in unit of pixels. |
| [`get_height_of_value(self)`](/cells/python-net/aspose.cells/cell/get_height_of_value/#) | Gets the height of the value in unit of pixels. |
| [`get_format_conditions(self)`](/cells/python-net/aspose.cells/cell/get_format_conditions/#) | Gets format conditions which applies to this cell. |
| [`get_formula(self, is_r1c1, is_local)`](/cells/python-net/aspose.cells/cell/get_formula/#bool-bool) | Get the formula of this cell. |
| [`get_precedents(self)`](/cells/python-net/aspose.cells/cell/get_precedents/#) | Gets all references appearing in this cell's formula. |
| [`get_dependents(self, is_all)`](/cells/python-net/aspose.cells/cell/get_dependents/#bool) | Get all cells whose formula references to this cell directly. |
| [`get_precedents_in_calculation(self)`](/cells/python-net/aspose.cells/cell/get_precedents_in_calculation/#) | Gets all precedents(reference to cells in current workbook) used by this cell's formula while calculating it. |
| [`get_dependents_in_calculation(self, recursive)`](/cells/python-net/aspose.cells/cell/get_dependents_in_calculation/#bool) | Gets all cells whose calculated result depends on this cell. |
| [`get_array_range(self)`](/cells/python-net/aspose.cells/cell/get_array_range/#) | Gets the array range if the cell's formula is an array formula. |
| [`remove_array_formula(self, leave_normal_formula)`](/cells/python-net/aspose.cells/cell/remove_array_formula/#bool) | Remove array formula. |
| [`copy(self, cell)`](/cells/python-net/aspose.cells/cell/copy/#aspose.cells.cell) | Copies data from a source cell. |
| [`characters(self, start_index, length)`](/cells/python-net/aspose.cells/cell/characters/#int-int) | Returns a Characters object that represents a range of characters within the cell text. |
| [`replace(self, place_holder, new_value, options)`](/cells/python-net/aspose.cells/cell/replace/#system.string-system.string-aspose.cells.replaceoptions) | Replace text of the cell with options. |
| [`insert_text(self, index, text)`](/cells/python-net/aspose.cells/cell/insert_text/#int-system.string) | Insert some characters to the cell.
| [`is_rich_text(self)`](/cells/python-net/aspose.cells/cell/is_rich_text/#) | Indicates whether the string value of this cell is a rich formatted text. |
| [`set_characters(self, characters)`](/cells/python-net/aspose.cells/cell/set_characters/#list) | Sets rich text format of the cell. |
| [`get_merged_range(self)`](/cells/python-net/aspose.cells/cell/get_merged_range/#) | Returns a [`Range`](/cells/python-net/aspose.cells/range) object which represents a merged range. |
| [`get_html_string(self, html5)`](/cells/python-net/aspose.cells/cell/get_html_string/#bool) | Gets the html string which contains data and some formats in this cell. |
| [`to_json(self)`](/cells/python-net/aspose.cells/cell/to_json/#) | Convert [`Cell`](/cells/python-net/aspose.cells/cell) to JSON struct data. |
| [`equals(self, cell)`](/cells/python-net/aspose.cells/cell/equals/#aspose.cells.cell) | Checks whether this object refers to the same cell with another cell object. |
| [`get_conditional_formatting_result(self)`](/cells/python-net/aspose.cells/cell/get_conditional_formatting_result/#) | Get the result of the conditional formatting. |
| [`get_validation(self)`](/cells/python-net/aspose.cells/cell/get_validation/#) | Gets the validation applied to this cell. |
| [`get_validation_value(self)`](/cells/python-net/aspose.cells/cell/get_validation_value/#) | Gets the value of validation which applied to this cell. |
| [`get_table(self)`](/cells/python-net/aspose.cells/cell/get_table/#) | Gets the table which contains this cell. |
| [`get_rich_value(self)`](/cells/python-net/aspose.cells/cell/get_rich_value/#) | Gets rich value of the cell. |
### Example
```python
from aspose.cells import TextAlignmentType, Workbook
from aspose.pydrawing import Color
excel = Workbook()
cells = excel.worksheets[0].cells
# Put a string into a cell
cell = cells.get(0, 0)
cell.put_value("Hello")
first = cell.string_value
# Put an integer into a cell
cell = cells.get("B1")
cell.put_value(12)
second = cell.int_value
# Put a double into a cell
cell = cells.get(0, 2)
cell.put_value(-1.234)
third = cell.double_value
# Put a formula into a cell
cell = cells.get("D1")
cell.formula = "=B1 + C1"
# Put a combined formula: "sum(average(b1,c1), b1)" to cell at b2
cell = cells.get("b2")
cell.formula = "=sum(average(b1,c1), b1)"
# Set style of a cell
style = cell.get_style()
# Set background color
style.background_color = Color.yellow
# Set format of a cell
style.font.name = "Courier New"
style.vertical_alignment = TextAlignmentType.TOP
cell.set_style(style)
```
### See Also
* module [`aspose.cells`](..)
* class [`Cell`](/cells/python-net/aspose.cells/cell)
* class [`Range`](/cells/python-net/aspose.cells/range)
