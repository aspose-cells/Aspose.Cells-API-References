##Cells class
## Cells class
Encapsulates a collection of cell relevant objects, such as [`Cell`](/cells/python-net/aspose.cells/cell), [`Row`](/cells/python-net/aspose.cells/row), ...etc.
The Cells type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [ods_cell_fields](/cells/python-net/aspose.cells/cells/ods_cell_fields) | Gets the list of fields of ods. |
| [count](/cells/python-net/aspose.cells/cells/count) | Gets the total count of instantiated Cell objects. |
| [count_large](/cells/python-net/aspose.cells/cells/count_large) | Gets the total count of instantiated Cell objects. |
| [rows](/cells/python-net/aspose.cells/cells/rows) | Gets the collection of [`Row`](/cells/python-net/aspose.cells/row) objects that represents the individual rows in this worksheet. |
| [merged_cells](/cells/python-net/aspose.cells/cells/merged_cells) | Gets the collection of merged cells. |
| [multi_thread_reading](/cells/python-net/aspose.cells/cells/multi_thread_reading) | Gets or sets whether the cells data model should support Multi-Thread reading.
| [memory_setting](/cells/python-net/aspose.cells/cells/memory_setting) | Gets or sets the memory usage option for this cells. |
| [style](/cells/python-net/aspose.cells/cells/style) | Gets and sets the default style of the worksheet. |
| [is_default_column_hidden](/cells/python-net/aspose.cells/cells/is_default_column_hidden) |  |
| [standard_width_inch](/cells/python-net/aspose.cells/cells/standard_width_inch) | Gets or sets the default column width in the worksheet, in unit of inches. |
| [standard_width_pixels](/cells/python-net/aspose.cells/cells/standard_width_pixels) | Gets or sets the default column width in the worksheet, in unit of pixels. |
| [standard_width](/cells/python-net/aspose.cells/cells/standard_width) | Gets or sets the default column width in the worksheet, in unit of characters. |
| [standard_height](/cells/python-net/aspose.cells/cells/standard_height) | Gets or sets the default row height in this worksheet, in unit of points. |
| [standard_height_pixels](/cells/python-net/aspose.cells/cells/standard_height_pixels) | Gets or sets the default row height in this worksheet, in unit of pixels. |
| [standard_height_inch](/cells/python-net/aspose.cells/cells/standard_height_inch) | Gets or sets the default row height in this worksheet, in unit of inches. |
| [preserve_string](/cells/python-net/aspose.cells/cells/preserve_string) | Gets or sets a value indicating whether all worksheet values are preserved as strings.
| [min_row](/cells/python-net/aspose.cells/cells/min_row) | Minimum row index of cell which contains data or style. |
| [max_row](/cells/python-net/aspose.cells/cells/max_row) | Maximum row index of cell which contains data or style. |
| [min_column](/cells/python-net/aspose.cells/cells/min_column) | Minimum column index of those cells that have been instantiated in the collection(does not include the column
| [max_column](/cells/python-net/aspose.cells/cells/max_column) | Maximum column index of those cells that have been instantiated in the collection(does not include the column
| [min_data_row](/cells/python-net/aspose.cells/cells/min_data_row) | Minimum row index of cell which contains data. |
| [max_data_row](/cells/python-net/aspose.cells/cells/max_data_row) | Maximum row index of cell which contains data. |
| [min_data_column](/cells/python-net/aspose.cells/cells/min_data_column) | Minimum column index of cell which contains data. |
| [max_data_column](/cells/python-net/aspose.cells/cells/max_data_column) | Maximum column index of cell which contains data. |
| [is_default_row_height_matched](/cells/python-net/aspose.cells/cells/is_default_row_height_matched) | Indicates that row height and default font height matches |
| [is_default_row_hidden](/cells/python-net/aspose.cells/cells/is_default_row_hidden) | Indicates whether the row is default hidden. |
| [columns](/cells/python-net/aspose.cells/cells/columns) | Gets the collection of [`Column`](/cells/python-net/aspose.cells/column) objects that represents the individual columns in this worksheet. |
| [ranges](/cells/python-net/aspose.cells/cells/ranges) | Gets the collection of [`Range`](/cells/python-net/aspose.cells/range) objects created at run time. |
| [last_cell](/cells/python-net/aspose.cells/cells/last_cell) | Gets the last cell in this worksheet. |
| [max_display_range](/cells/python-net/aspose.cells/cells/max_display_range) | Gets the max range which includes data, merged cells and shapes. |
| [first_cell](/cells/python-net/aspose.cells/cells/first_cell) | Gets the first cell in this worksheet. |
### Methods
| Method | Description |
| :- | :- |
| [`create_range(self, upper_left_cell, lower_right_cell)`](/cells/python-net/aspose.cells/cells/create_range/#system.string-system.string) | Creates a [`Range`](/cells/python-net/aspose.cells/range) object from a range of cells. |
| [`create_range(self, first_row, first_column, total_rows, total_columns)`](/cells/python-net/aspose.cells/cells/create_range/#int-int-int-int) | Creates a [`Range`](/cells/python-net/aspose.cells/range) object from a range of cells. |
| [`create_range(self, address)`](/cells/python-net/aspose.cells/cells/create_range/#system.string) | Creates a [`Range`](/cells/python-net/aspose.cells/range) object from an address of the range. |
| [`create_range(self, first_index, number, is_vertical)`](/cells/python-net/aspose.cells/cells/create_range/#int-int-bool) | Creates a [`Range`](/cells/python-net/aspose.cells/range) object from rows of cells or columns of cells. |
| [`get(self, row, column)`](/cells/python-net/aspose.cells/cells/get/#int-int) | Add API for Python Via .Net.since this[int row, int column] is unsupported |
| [`get(self, cell_name)`](/cells/python-net/aspose.cells/cells/get/#system.string) | Add API for Python Via .Net.since this[string cellName] is unsupported |
| [`import_object_array(self, obj_array, first_row, first_column, is_vertical)`](/cells/python-net/aspose.cells/cells/import_object_array/#list-int-int-bool) | Imports an array of data into a worksheet. |
| [`import_object_array(self, obj_array, first_row, first_column, is_vertical, skip)`](/cells/python-net/aspose.cells/cells/import_object_array/#list-int-int-bool-int) | Imports an array of data into a worksheet. |
| [`import_array(self, string_array, first_row, first_column, is_vertical)`](/cells/python-net/aspose.cells/cells/import_array/#list-int-int-bool) | Imports an array of string into a worksheet. |
| [`import_array(self, int_array, first_row, first_column, is_vertical)`](/cells/python-net/aspose.cells/cells/import_array/#list-int-int-bool) | Imports an array of integer into a worksheet. |
| [`import_array(self, double_array, first_row, first_column, is_vertical)`](/cells/python-net/aspose.cells/cells/import_array/#list-int-int-bool) | Imports an array of double into a worksheet. |
| [`import_csv(self, file_name, splitter, convert_numeric_data, first_row, first_column)`](/cells/python-net/aspose.cells/cells/import_csv/#system.string-system.string-bool-int-int) | Import a CSV file to the cells. |
| [`import_csv(self, stream, splitter, convert_numeric_data, first_row, first_column)`](/cells/python-net/aspose.cells/cells/import_csv/#io.rawiobase-system.string-bool-int-int) | Import a CSV file to the cells. |
| [`import_csv(self, file_name, options, first_row, first_column)`](/cells/python-net/aspose.cells/cells/import_csv/#system.string-aspose.cells.txtloadoptions-int-int) | Import a CSV file to the cells. |
| [`import_csv(self, stream, options, first_row, first_column)`](/cells/python-net/aspose.cells/cells/import_csv/#io.rawiobase-aspose.cells.txtloadoptions-int-int) | Import a CSV file to the cells. |
| [`merge(self, first_row, first_column, total_rows, total_columns)`](/cells/python-net/aspose.cells/cells/merge/#int-int-int-int) | Merges a specified range of cells into a single cell. |
| [`merge(self, first_row, first_column, total_rows, total_columns, merge_conflict)`](/cells/python-net/aspose.cells/cells/merge/#int-int-int-int-bool) | Merges a specified range of cells into a single cell. |
| [`merge(self, first_row, first_column, total_rows, total_columns, check_conflict, merge_conflict)`](/cells/python-net/aspose.cells/cells/merge/#int-int-int-int-bool-bool) | Merges a specified range of cells into a single cell. |
| [`get_row_height(self, row, is_original, unit_type)`](/cells/python-net/aspose.cells/cells/get_row_height/#int-bool-aspose.cells.cellsunittype) | Gets row's height. |
| [`get_row_height(self, row)`](/cells/python-net/aspose.cells/cells/get_row_height/#int) | Gets the height of a specified row, in unit of points. |
| [`get_column_width(self, column, is_original, unit_type)`](/cells/python-net/aspose.cells/cells/get_column_width/#int-bool-aspose.cells.cellsunittype) | Gets the column width. |
| [`get_column_width(self, column)`](/cells/python-net/aspose.cells/cells/get_column_width/#int) | Gets the width(in unit of characters) of the specified column in normal view |
| [`get_column_width_pixel(self, column)`](/cells/python-net/aspose.cells/cells/get_column_width_pixel/#int) | Gets the width of the specified column in normal view, in units of pixel. |
| [`get_column_width_pixel(self, column, original)`](/cells/python-net/aspose.cells/cells/get_column_width_pixel/#int-bool) | Gets the width of the specified column in normal view, in units of pixel. |
| [`copy_columns(self, source_cells0, source_column_index, destination_column_index, column_number, paste_options)`](/cells/python-net/aspose.cells/cells/copy_columns/#aspose.cells.cells-int-int-int-aspose.cells.pasteoptions) | Copies data and formats of a whole column. |
| [`copy_columns(self, source_cells0, source_column_index, destination_column_index, column_number)`](/cells/python-net/aspose.cells/cells/copy_columns/#aspose.cells.cells-int-int-int) | Copies data and formats of a whole column. |
| [`copy_columns(self, source_cells, source_column_index, source_total_columns, destination_column_index, destination_total_columns)`](/cells/python-net/aspose.cells/cells/copy_columns/#aspose.cells.cells-int-int-int-int) | Copies data and formats of the whole columns. |
| [`copy_rows(self, source_cells, source_row_index, destination_row_index, row_number)`](/cells/python-net/aspose.cells/cells/copy_rows/#aspose.cells.cells-int-int-int) | Copies data and formats of some whole rows. |
| [`copy_rows(self, source_cells0, source_row_index, destination_row_index, row_number, copy_options)`](/cells/python-net/aspose.cells/cells/copy_rows/#aspose.cells.cells-int-int-int-aspose.cells.copyoptions) | Copies data and formats of some whole rows. |
| [`copy_rows(self, source_cells0, source_row_index, destination_row_index, row_number, copy_options, paste_options)`](/cells/python-net/aspose.cells/cells/copy_rows/#aspose.cells.cells-int-int-int-aspose.cells.copyoptions-aspose.cells.pasteoptions) | Copies data and formats of some whole rows. |
| [`group_columns(self, first_index, last_index)`](/cells/python-net/aspose.cells/cells/group_columns/#int-int) | Groups columns. |
| [`group_columns(self, first_index, last_index, is_hidden)`](/cells/python-net/aspose.cells/cells/group_columns/#int-int-bool) | Groups columns. |
| [`ungroup_rows(self, first_index, last_index, is_all)`](/cells/python-net/aspose.cells/cells/ungroup_rows/#int-int-bool) | Ungroups rows. |
| [`ungroup_rows(self, first_index, last_index)`](/cells/python-net/aspose.cells/cells/ungroup_rows/#int-int) | Ungroups rows. |
| [`group_rows(self, first_index, last_index, is_hidden)`](/cells/python-net/aspose.cells/cells/group_rows/#int-int-bool) | Groups rows. |
| [`group_rows(self, first_index, last_index)`](/cells/python-net/aspose.cells/cells/group_rows/#int-int) | Groups rows. |
| [`delete_column(self, column_index, update_reference)`](/cells/python-net/aspose.cells/cells/delete_column/#int-bool) | Deletes a column. |
| [`delete_column(self, column_index)`](/cells/python-net/aspose.cells/cells/delete_column/#int) | Deletes a column. |
| [`delete_columns(self, column_index, total_columns, update_reference)`](/cells/python-net/aspose.cells/cells/delete_columns/#int-int-bool) | Deletes several columns. |
| [`delete_columns(self, column_index, total_columns, options)`](/cells/python-net/aspose.cells/cells/delete_columns/#int-int-aspose.cells.deleteoptions) | Deletes several columns. |
| [`delete_row(self, row_index)`](/cells/python-net/aspose.cells/cells/delete_row/#int) | Deletes a row. |
| [`delete_row(self, row_index, update_reference)`](/cells/python-net/aspose.cells/cells/delete_row/#int-bool) | Deletes a row. |
| [`delete_rows(self, row_index, total_rows)`](/cells/python-net/aspose.cells/cells/delete_rows/#int-int) | Deletes multiple rows. |
| [`delete_rows(self, row_index, total_rows, update_reference)`](/cells/python-net/aspose.cells/cells/delete_rows/#int-int-bool) | Deletes multiple rows in the worksheet. |
| [`delete_rows(self, row_index, total_rows, options)`](/cells/python-net/aspose.cells/cells/delete_rows/#int-int-aspose.cells.deleteoptions) | Deletes multiple rows in the worksheet. |
| [`delete_blank_columns(self)`](/cells/python-net/aspose.cells/cells/delete_blank_columns/#) | Delete all blank columns which do not contain any data. |
| [`delete_blank_columns(self, options)`](/cells/python-net/aspose.cells/cells/delete_blank_columns/#aspose.cells.deleteoptions) | Delete all blank columns which do not contain any data. |
| [`delete_blank_rows(self)`](/cells/python-net/aspose.cells/cells/delete_blank_rows/#) | Delete all blank rows which do not contain any data or other object. |
| [`delete_blank_rows(self, options)`](/cells/python-net/aspose.cells/cells/delete_blank_rows/#aspose.cells.deleteoptions) | Delete all blank rows which do not contain any data or some special objects such as visible comment, pivot table. |
| [`insert_columns(self, column_index, total_columns)`](/cells/python-net/aspose.cells/cells/insert_columns/#int-int) | Inserts some columns into the worksheet. |
| [`insert_columns(self, column_index, total_columns, update_reference)`](/cells/python-net/aspose.cells/cells/insert_columns/#int-int-bool) | Inserts some columns into the worksheet. |
| [`insert_columns(self, column_index, total_columns, options)`](/cells/python-net/aspose.cells/cells/insert_columns/#int-int-aspose.cells.insertoptions) | Inserts some columns into the worksheet. |
| [`insert_column(self, column_index, update_reference)`](/cells/python-net/aspose.cells/cells/insert_column/#int-bool) | Inserts a new column into the worksheet. |
| [`insert_column(self, column_index)`](/cells/python-net/aspose.cells/cells/insert_column/#int) | Inserts a new column into the worksheet. |
| [`insert_rows(self, row_index, total_rows, update_reference)`](/cells/python-net/aspose.cells/cells/insert_rows/#int-int-bool) | Inserts multiple rows into the worksheet. |
| [`insert_rows(self, row_index, total_rows, options)`](/cells/python-net/aspose.cells/cells/insert_rows/#int-int-aspose.cells.insertoptions) | Inserts multiple rows into the worksheet. |
| [`insert_rows(self, row_index, total_rows)`](/cells/python-net/aspose.cells/cells/insert_rows/#int-int) | Inserts multiple rows into the worksheet. |
| [`clear_range(self, range)`](/cells/python-net/aspose.cells/cells/clear_range/#aspose.cells.cellarea) | Clears contents and formatting of a range. |
| [`clear_range(self, start_row, start_column, end_row, end_column)`](/cells/python-net/aspose.cells/cells/clear_range/#int-int-int-int) | Clears contents and formatting of a range. |
| [`clear_contents(self, range)`](/cells/python-net/aspose.cells/cells/clear_contents/#aspose.cells.cellarea) | Clears contents of a range. |
| [`clear_contents(self, start_row, start_column, end_row, end_column)`](/cells/python-net/aspose.cells/cells/clear_contents/#int-int-int-int) | Clears contents of a range. |
| [`clear_formats(self, range)`](/cells/python-net/aspose.cells/cells/clear_formats/#aspose.cells.cellarea) | Clears formatting of a range. |
| [`clear_formats(self, start_row, start_column, end_row, end_column)`](/cells/python-net/aspose.cells/cells/clear_formats/#int-int-int-int) | Clears formatting of a range. |
| [`find(self, what, previous_cell)`](/cells/python-net/aspose.cells/cells/find/#system.object-aspose.cells.cell) | Finds the cell containing with the input object. |
| [`find(self, what, previous_cell, find_options)`](/cells/python-net/aspose.cells/cells/find/#system.object-aspose.cells.cell-aspose.cells.findoptions) | Finds the cell containing with the input object. |
| [`end_cell_in_row(self, row_index)`](/cells/python-net/aspose.cells/cells/end_cell_in_row/#int) | Gets the last cell in this row. |
| [`end_cell_in_row(self, start_row, end_row, start_column, end_column)`](/cells/python-net/aspose.cells/cells/end_cell_in_row/#int-int-int-int) | Gets the last cell with maximum row index in this range. |
| [`end_cell_in_column(self, column_index)`](/cells/python-net/aspose.cells/cells/end_cell_in_column/#int) | Gets the last cell in this column. |
| [`end_cell_in_column(self, start_row, end_row, start_column, end_column)`](/cells/python-net/aspose.cells/cells/end_cell_in_column/#int-int-int-int) | Gets the last cell with maximum column index in this range. |
| [`insert_range(self, area, shift_number, shift_type, update_reference)`](/cells/python-net/aspose.cells/cells/insert_range/#aspose.cells.cellarea-int-aspose.cells.shifttype-bool) | Inserts a range of cells and shift cells according to the shift option. |
| [`insert_range(self, area, shift_type)`](/cells/python-net/aspose.cells/cells/insert_range/#aspose.cells.cellarea-aspose.cells.shifttype) | Inserts a range of cells and shift cells according to the shift option. |
| [`insert_range(self, area, shift_number, shift_type)`](/cells/python-net/aspose.cells/cells/insert_range/#aspose.cells.cellarea-int-aspose.cells.shifttype) | Inserts a range of cells and shift cells according to the shift option. |
| [`import_custom_objects(self, list, property_names, is_property_name_shown, first_row, first_column, row_number, insert_rows, date_format_string, convert_string_to_number)`](/cells/python-net/aspose.cells/cells/import_custom_objects/#list-list-bool-int-int-int-bool-system.string-bool) | Imports custom objects. |
| [`import_custom_objects(self, list, first_row, first_column, options)`](/cells/python-net/aspose.cells/cells/import_custom_objects/#list-int-int-aspose.cells.importtableoptions) | Imports custom objects. |
| [`subtotal(self, ca, group_by, function, total_list)`](/cells/python-net/aspose.cells/cells/subtotal/#aspose.cells.cellarea-int-aspose.cells.consolidationfunction-list) | Creates subtotals for the range. |
| [`subtotal(self, ca, group_by, function, total_list, replace, page_breaks, summary_below_data)`](/cells/python-net/aspose.cells/cells/subtotal/#aspose.cells.cellarea-int-aspose.cells.consolidationfunction-list-bool-bool-bool) | Creates subtotals for the range. |
| [`remove_duplicates(self)`](/cells/python-net/aspose.cells/cells/remove_duplicates/#) | Removes duplicate rows in the sheet. |
| [`remove_duplicates(self, start_row, start_column, end_row, end_column)`](/cells/python-net/aspose.cells/cells/remove_duplicates/#int-int-int-int) | Removes duplicate values in the range. |
| [`remove_duplicates(self, start_row, start_column, end_row, end_column, has_headers, column_offsets)`](/cells/python-net/aspose.cells/cells/remove_duplicates/#int-int-int-int-bool-list) | Removes duplicate data of the range. |
| [`get_cell_display_style(self, row, column)`](/cells/python-net/aspose.cells/cells/get_cell_display_style/#int-int) | Get the display style of given cell. |
| [`get_cell_display_style(self, row, column, adjacent_borders)`](/cells/python-net/aspose.cells/cells/get_cell_display_style/#int-int-aspose.cells.bordertype) | Get the display style of given cell. |
| [`get_row_enumerator(self)`](/cells/python-net/aspose.cells/cells/get_row_enumerator/#) | Gets the rows enumerator. |
| [`get_merged_areas(self)`](/cells/python-net/aspose.cells/cells/get_merged_areas/#) | Gets all merged cells. |
| [`get_cell(self, row, column)`](/cells/python-net/aspose.cells/cells/get_cell/#int-int) | Gets the [`Cell`](/cells/python-net/aspose.cells/cell) element or null at the specified cell row index and column index. |
| [`get_row(self, row)`](/cells/python-net/aspose.cells/cells/get_row/#int) | Gets the [`Row`](/cells/python-net/aspose.cells/row) element at the specified cell row index. |
| [`check_cell(self, row, column)`](/cells/python-net/aspose.cells/cells/check_cell/#int-int) | Gets the [`Cell`](/cells/python-net/aspose.cells/cell) element or null at the specified cell row index and column index. |
| [`check_row(self, row)`](/cells/python-net/aspose.cells/cells/check_row/#int) | Gets the [`Row`](/cells/python-net/aspose.cells/row) element or null at the specified cell row index. |
| [`check_column(self, column_index)`](/cells/python-net/aspose.cells/cells/check_column/#int) | Gets the [`Column`](/cells/python-net/aspose.cells/column) element or null at the specified column index. |
| [`is_row_hidden(self, row_index)`](/cells/python-net/aspose.cells/cells/is_row_hidden/#int) | Checks whether a row at given index is hidden. |
| [`is_column_hidden(self, column_index)`](/cells/python-net/aspose.cells/cells/is_column_hidden/#int) | Checks whether a column at given index is hidden. |
| [`add_range(self, range_object)`](/cells/python-net/aspose.cells/cells/add_range/#aspose.cells.range) | Adds a range object reference to cells |
| [`clear(self)`](/cells/python-net/aspose.cells/cells/clear/#) | Clears all data of the worksheet. |
| [`import_data(self, table, first_row, first_column, options)`](/cells/python-net/aspose.cells/cells/import_data/#aspose.cells.icellsdatatable-int-int-aspose.cells.importtableoptions) | Import data from custom data table. |
| [`import_array_list(self, array_list, first_row, first_column, is_vertical)`](/cells/python-net/aspose.cells/cells/import_array_list/#list-int-int-bool) | Imports an arraylist of data into a worksheet. |
| [`import_formula_array(self, string_array, first_row, first_column, is_vertical)`](/cells/python-net/aspose.cells/cells/import_formula_array/#list-int-int-bool) | Imports an array of formula into a worksheet. |
| [`text_to_columns(self, row, column, total_rows, options)`](/cells/python-net/aspose.cells/cells/text_to_columns/#int-int-int-aspose.cells.txtloadoptions) | Splits content in specified column into multiple columns.. |
| [`un_merge(self, first_row, first_column, total_rows, total_columns)`](/cells/python-net/aspose.cells/cells/un_merge/#int-int-int-int) | Unmerges a specified range of merged cells. |
| [`clear_merged_cells(self)`](/cells/python-net/aspose.cells/cells/clear_merged_cells/#) | Clears all merged ranges. |
| [`hide_row(self, row)`](/cells/python-net/aspose.cells/cells/hide_row/#int) | Hides a row. |
| [`unhide_row(self, row, height)`](/cells/python-net/aspose.cells/cells/unhide_row/#int-float) | Unhides a row. |
| [`hide_rows(self, row, total_rows)`](/cells/python-net/aspose.cells/cells/hide_rows/#int-int) | Hides multiple rows. |
| [`unhide_rows(self, row, total_rows, height)`](/cells/python-net/aspose.cells/cells/unhide_rows/#int-int-float) | Unhides the hidden rows. |
| [`set_row_height_pixel(self, row, pixels)`](/cells/python-net/aspose.cells/cells/set_row_height_pixel/#int-int) | Sets row height in unit of pixels. |
| [`set_row_height_inch(self, row, inches)`](/cells/python-net/aspose.cells/cells/set_row_height_inch/#int-float) | Sets row height in unit of inches. |
| [`set_row_height(self, row, height)`](/cells/python-net/aspose.cells/cells/set_row_height/#int-float) | Sets the height of the specified row. |
| [`get_row_original_height_point(self, row)`](/cells/python-net/aspose.cells/cells/get_row_original_height_point/#int) | Gets original row's height in unit of point if the row is hidden |
| [`get_column_original_width_point(self, column)`](/cells/python-net/aspose.cells/cells/get_column_original_width_point/#int) | Gets original column's height in unit of point if the column is hidden |
| [`hide_column(self, column)`](/cells/python-net/aspose.cells/cells/hide_column/#int) | Hides a column. |
| [`unhide_column(self, column, width)`](/cells/python-net/aspose.cells/cells/unhide_column/#int-float) | Unhides a column |
| [`hide_columns(self, column, total_columns)`](/cells/python-net/aspose.cells/cells/hide_columns/#int-int) | Hide multiple columns. |
| [`unhide_columns(self, column, total_columns, width)`](/cells/python-net/aspose.cells/cells/unhide_columns/#int-int-float) | Unhide multiple columns. |
| [`get_view_row_height(self, row)`](/cells/python-net/aspose.cells/cells/get_view_row_height/#int) | Gets the height of a specified row. |
| [`get_row_height_inch(self, row)`](/cells/python-net/aspose.cells/cells/get_row_height_inch/#int) | Gets the height of a specified row in unit of inches. |
| [`get_view_row_height_inch(self, row)`](/cells/python-net/aspose.cells/cells/get_view_row_height_inch/#int) | Gets the height of a specified row in unit of inches. |
| [`get_row_height_pixel(self, row)`](/cells/python-net/aspose.cells/cells/get_row_height_pixel/#int) | Gets the height of a specified row in unit of pixel. |
| [`set_column_width_pixel(self, column, pixels)`](/cells/python-net/aspose.cells/cells/set_column_width_pixel/#int-int) | Sets column width in unit of pixels in normal view. |
| [`set_column_width_inch(self, column, inches)`](/cells/python-net/aspose.cells/cells/set_column_width_inch/#int-float) | Sets column width in unit of inches  in normal view. |
| [`set_column_width(self, column, width)`](/cells/python-net/aspose.cells/cells/set_column_width/#int-float) | Sets the width of the specified column in normal view. |
| [`get_column_width_inch(self, column)`](/cells/python-net/aspose.cells/cells/get_column_width_inch/#int) | Gets the width of the specified column in normal view, in units of inches. |
| [`get_view_column_width_pixel(self, column)`](/cells/python-net/aspose.cells/cells/get_view_column_width_pixel/#int) | Get the width in different view type. |
| [`set_view_column_width_pixel(self, column, pixels)`](/cells/python-net/aspose.cells/cells/set_view_column_width_pixel/#int-int) | Sets the width of the column in different view. |
| [`get_last_data_row(self, column)`](/cells/python-net/aspose.cells/cells/get_last_data_row/#int) | Gets the last row index of cell which contains data in the specified column. |
| [`get_first_data_row(self, column)`](/cells/python-net/aspose.cells/cells/get_first_data_row/#int) | Gets the first row index of cell which contains data in the specified column. |
| [`apply_column_style(self, column, style, flag)`](/cells/python-net/aspose.cells/cells/apply_column_style/#int-aspose.cells.style-aspose.cells.styleflag) | Applies formats for a whole column. |
| [`apply_row_style(self, row, style, flag)`](/cells/python-net/aspose.cells/cells/apply_row_style/#int-aspose.cells.style-aspose.cells.styleflag) | Applies formats for a whole row. |
| [`apply_style(self, style, flag)`](/cells/python-net/aspose.cells/cells/apply_style/#aspose.cells.style-aspose.cells.styleflag) | Applies formats for a whole worksheet. |
| [`copy_column(self, source_cells, source_column_index, destination_column_index)`](/cells/python-net/aspose.cells/cells/copy_column/#aspose.cells.cells-int-int) | Copies data and formats of a whole column. |
| [`copy_row(self, source_cells, source_row_index, destination_row_index)`](/cells/python-net/aspose.cells/cells/copy_row/#aspose.cells.cells-int-int) | Copies data and formats of a whole row. |
| [`get_grouped_row_outline_level(self, row_index)`](/cells/python-net/aspose.cells/cells/get_grouped_row_outline_level/#int) | Gets the outline level (zero-based) of the row. |
| [`get_grouped_column_outline_level(self, column_index)`](/cells/python-net/aspose.cells/cells/get_grouped_column_outline_level/#int) | Gets the outline level (zero-based) of the column. |
| [`get_max_grouped_column_outline_level(self)`](/cells/python-net/aspose.cells/cells/get_max_grouped_column_outline_level/#) | Gets the max grouped column outline level (zero-based). |
| [`get_max_grouped_row_outline_level(self)`](/cells/python-net/aspose.cells/cells/get_max_grouped_row_outline_level/#) | Gets the max grouped row outline level (zero-based). |
| [`show_group_detail(self, is_vertical, index)`](/cells/python-net/aspose.cells/cells/show_group_detail/#bool-int) | Expands the grouped rows/columns. |
| [`hide_group_detail(self, is_vertical, index)`](/cells/python-net/aspose.cells/cells/hide_group_detail/#bool-int) | Collapses the grouped rows/columns. |
| [`ungroup_columns(self, first_index, last_index)`](/cells/python-net/aspose.cells/cells/ungroup_columns/#int-int) | Ungroups columns. |
| [`is_deleting_range_enabled(self, start_row, start_column, total_rows, total_columns)`](/cells/python-net/aspose.cells/cells/is_deleting_range_enabled/#int-int-int-int) | Check whether the range could be deleted. |
| [`is_blank_column(self, column_index)`](/cells/python-net/aspose.cells/cells/is_blank_column/#int) | Checks whether given column is blank(does not contain any data). |
| [`insert_row(self, row_index)`](/cells/python-net/aspose.cells/cells/insert_row/#int) | Inserts a new row into the worksheet. |
| [`link_to_xml_map(self, map_name, row, column, path)`](/cells/python-net/aspose.cells/cells/link_to_xml_map/#system.string-int-int-system.string) | Link to a xml map. |
| [`move_range(self, source_area, dest_row, dest_column)`](/cells/python-net/aspose.cells/cells/move_range/#aspose.cells.cellarea-int-int) | Moves the range. |
| [`insert_cut_cells(self, cut_range, row, column, shift_type)`](/cells/python-net/aspose.cells/cells/insert_cut_cells/#aspose.cells.range-int-int-aspose.cells.shifttype) | Insert cut range. |
| [`delete_range(self, start_row, start_column, end_row, end_column, shift_type)`](/cells/python-net/aspose.cells/cells/delete_range/#int-int-int-int-aspose.cells.shifttype) | Deletes a range of cells and shift cells according to the shift option. |
| [`retrieve_subtotal_setting(self, ca)`](/cells/python-net/aspose.cells/cells/retrieve_subtotal_setting/#aspose.cells.cellarea) | Retrieves subtotals setting of the range. |
| [`remove_formulas(self)`](/cells/python-net/aspose.cells/cells/remove_formulas/#) | Removes all formula and replaces with the value of the formula. |
| [`convert_string_to_numeric_value(self)`](/cells/python-net/aspose.cells/cells/convert_string_to_numeric_value/#) | Converts all string data in the worksheet to numeric value if possible. |
| [`get_dependents(self, is_all, row, column)`](/cells/python-net/aspose.cells/cells/get_dependents/#bool-int-int) | Get all cells which refer to the specific cell. |
| [`get_dependents_in_calculation(self, row, column, recursive)`](/cells/python-net/aspose.cells/cells/get_dependents_in_calculation/#int-int-bool) | Gets all cells whose calculated result depends on specific cell. |
| [`get_cells_with_place_in_cell_picture(self)`](/cells/python-net/aspose.cells/cells/get_cells_with_place_in_cell_picture/#) | Gets all cells that contain embedded picture. |
| [`get_cell_style(self, row, column)`](/cells/python-net/aspose.cells/cells/get_cell_style/#int-int) | Get the style of given cell. |
### Remarks
### See Also
* module [`aspose.cells`](..)
* class [`Cell`](/cells/python-net/aspose.cells/cell)
* class [`Column`](/cells/python-net/aspose.cells/column)
* class [`Range`](/cells/python-net/aspose.cells/range)
* class [`Row`](/cells/python-net/aspose.cells/row)
