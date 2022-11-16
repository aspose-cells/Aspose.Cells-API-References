---
title: Cell
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 140
url: /python-net/aspose.cells/cell/
---

## Cell class

Encapsulates the object that represents a single Workbook cell.

The Cell type exposes the following members:
## Properties
| Name | Description |
| :- | :- |
|worksheet|Gets the parent worksheet.|
|date_time_value|Gets the DateTime value contained in the cell.|
|row|Gets row number (zero based) of the cell.|
|column|Gets column number (zero based) of the cell.|
|is_formula|Represents if the specified cell contains formula.|
|type|Represents cell value type.|
|name|Gets the name of the cell.|
|is_error_value|Checks if the value of this cell is an error.|
|is_numeric_value|Indicates whether the inner value of this cell is numeric(int, double and datetime)|
|string_value|Gets the string value contained in the cell. If the type of this cell is string, then return the string value itself.<br/>            For other cell types, the formatted string value (formatted with the specified style of this cell) will be returned.<br/>            The formatted cell value is same with what you can get from excel when copying a cell as text(such as<br/>            copying cell to text editor or exporting to csv).|
|string_value_without_format|Gets cell's value as string without any format.|
|number_category_type|Represents the category type of this cell's number formatting.|
|display_string_value|Gets the formatted string value of this cell by cell's display style.|
|int_value|Gets the integer value contained in the cell.|
|double_value|Gets the double value contained in the cell.|
|float_value|Gets the float value contained in the cell.|
|bool_value|Gets the boolean value contained in the cell.|
|shared_style_index|Gets cell's shared style index in the style pool.|
|formula|Gets or sets a formula of the [Cell](/cells/python-net/aspose.cells/cell/).|
|formula_local|Get the locale formatted formula of the cell.|
|r1c1_formula|Gets or sets a R1C1 formula of the [Cell](/cells/python-net/aspose.cells/cell/).|
|contains_external_link|Indicates whether this cell contains an external link.<br/>            Only applies when the cell is a formula cell.|
|is_array_header|Indicates the cell's formula is and array formula <br/>            and it is the first cell of the array.|
|is_array_formula|Indicates whether the cell formula is an array formula.|
|is_in_array|Indicates whether the cell formula is an array formula.|
|is_shared_formula|Indicates whether the cell formula is part of shared formula.|
|is_table_formula|Indicates whether this cell is part of table formula.|
|is_in_table|Indicates whether this cell is part of table formula.|
|value|Gets the value contained in this cell.|
|is_style_set|Indicates if the cell's style is set. If return false, it means this cell has a default cell format.|
|is_merged|Checks if a cell is part of a merged range or not.|
|comment|Gets the comment of this cell.|
|html_string|Gets and sets the html string which contains data and some formats in this cell.|
## Methods
| Name | Description |
| :- | :- |
|calculate(options)|Calculates the formula of the cell.|
|calculate(ignore_error, custom_function)|Calculates the formula of the cell.|
|put_value(bool_value)|Puts a boolean value into the cell.|
|put_value(int_value)|Puts an integer value into the cell.|
|put_value(double_value)|Puts a double value into the cell.|
|put_value(string_value, is_converted, set_style)|Puts a value into the cell, if appropriate the value will be converted to other data type and cell's number format will be reset.|
|put_value(string_value, is_converted)|Puts a value into the cell, if appropriate the value will be converted to other data type and cell's number format will be reset.|
|put_value(string_value)|Puts a value into the cell, if appropriate the value will be converted to other data type and cell's number format will be reset.|
|put_value(date_time)|Puts a DateTime value into the cell.|
|put_value(object_value)|Puts an object value into the cell.|
|get_display_style()|Gets the display style of the cell.<br/>            If this cell is also affected by other settings such as conditional formatting, list objects, etc.,<br/>            then the display style may be different from cell.GetStyle().|
|get_display_style(include_merged_borders)|Gets the display style of the cell.<br/>            If the cell is conditional formatted, the display style is not same as the cell.GetStyle().|
|get_style()|Gets the cell style.|
|get_style(check_borders)|If checkBorders is true, check whether other cells' borders will effect the style of this cell.|
|set_style(style)|Sets the cell style.|
|set_style(style, explicit_flag)|Apply the cell style.|
|set_style(style, flag)|Apply the cell style.|
|set_formula(formula, value)|Set the formula and the value of the formula.|
|set_formula(formula, is_r1c1, is_local, value)|Set the formula and the value of the formula.|
|set_formula(formula, options, value)|Set the formula and the value of the formula.|
|set_array_formula(array_formula, row_number, column_number, is_r1c1, is_local)|Sets an array formula to a range of cells.|
|set_array_formula(array_formula, row_number, column_number)|Sets an array formula to a range of cells.|
|set_array_formula(array_formula, row_number, column_number, options)|Sets an array formula to a range of cells.|
|set_array_formula(array_formula, row_number, column_number, options, values)|Sets an array formula to a range of cells.|
|set_shared_formula(shared_formula, row_number, column_number, is_r1c1, is_local)|Sets a formula to a range of cells.|
|set_shared_formula(shared_formula, row_number, column_number)|Sets a formula to a range of cells.|
|set_shared_formula(shared_formula, row_number, column_number, options)|Sets shared formulas to a range of cells.|
|set_shared_formula(shared_formula, row_number, column_number, options, values)|Sets shared formulas to a range of cells.|
|get_leafs()|Get all cells which reference to this cell directly and need to be updated when this cell is modified.|
|get_leafs(recursive)|Get all cells which will be updated when this cell is modified.|
|set_dynamic_array_formula(array_formula, options, calculate_value)|Sets dynamic array formula and make the formula spill into neighboring cells if possible.|
|set_dynamic_array_formula(array_formula, options, values, calculate_range, calculate_value)|Sets dynamic array formula and make the formula spill into neighboring cells if possible.|
|set_dynamic_array_formula(array_formula, options, values, calculate_range, calculate_value, copts)|Sets dynamic array formula and make the formula spill into neighboring cells if possible.|
|set_table_formula(row_number, column_number, row_input_cell, column_input_cell, values)|Create two-variable data table for given range starting from this cell.|
|set_table_formula(row_number, column_number, input_cell, is_row_input, values)|Create one-variable data table for given range starting from this cell.|
|set_table_formula(row_number, column_number, row_index_of_row_input_cell, column_index_of_row_input_cell, row_index_of_column_input_cell, column_index_of_column_input_cell, values)|Create two-variable data table for given range starting from this cell.|
|set_table_formula(row_number, column_number, row_index_of_input_cell, column_index_of_input_cell, is_row_input, values)|Create one-variable data table for given range starting from this cell.|
|get_characters()|Returns all Characters objects <br/>            that represents a range of characters within the cell text.|
|get_characters(flag)|Returns all Characters objects <br/>            that represents a range of characters within the cell text.|
|get_string_value(format_strategy)|Gets the string value by specific formatted strategy.|
|get_width_of_value()|Gets the width of the value in unit of pixels.|
|get_height_of_value()|Gets the height of the value in unit of pixels.|
|get_format_conditions()|Gets format conditions which applies to this cell.|
|get_formula(is_r1c1, is_local)|Get the formula of this cell.|
|get_precedents()|Gets all references appearing in this cell's formula.|
|get_dependents(is_all)|Get all cells whose formula references to this cell directly.|
|get_precedents_in_calculation()|Gets all precedents(reference to cells in current workbook) used by this cell's formula while calculating it.|
|get_dependents_in_calculation(recursive)|Gets all cells whose calculated result depends on this cell.|
|get_array_range()|Gets the array range if the cell's formula is an array formula.|
|remove_array_formula(leave_normal_formula)|Remove array formula.|
|copy(cell)|Copies data from a source cell.|
|characters(start_index, length)|Returns a Characters object that represents a range of characters within the cell text.|
|is_rich_text()|Indicates whether the cell string value is a rich text.|
|set_characters(characters)|Sets rich text format of the cell.|
|get_merged_range()|Returns a [Range](/cells/python-net/aspose.cells/range/) object which represents a merged range.|
|get_html_string(html5)|Gets the html string which contains data and some formats in this cell.|
|equals(cell)|Checks whether this object refers to the same cell with another.|
|get_conditional_formatting_result()|Get the result of the conditional formatting.|
|get_validation()|Gets the validation applied to this cell.|
|get_validation_value()|Gets the value of validation which applied to this cell.|
|get_table()|Gets the table which contains this cell.|

### See Also

* namespace [aspose.cells](/cells/python-net/aspose.cells/)
* assembly [Aspose.Cells](/cells/python-net/)

