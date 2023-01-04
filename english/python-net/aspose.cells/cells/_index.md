---
title: Cells class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 180
url: /python-net/aspose.cells/cells/
is_root: false
---

## Cells class

Encapsulates a collection of cell relevant objects, such as [Cell](/cells/python-net/aspose.cells/cell), [Row](/cells/python-net/aspose.cells/row), ...etc.



The Cells type exposes the following members:

### Properties
| Property | Description |
| :- | :- |
| [ods_cell_fields](/cells/python-net/aspose.cells/cells/ods_cell_fields) | Gets the list of fields of ods. |
| [count](/cells/python-net/aspose.cells/cells/count) | Gets the total count of instantiated Cell objects. |
| [count_large](/cells/python-net/aspose.cells/cells/count_large) | Gets the total count of instantiated Cell objects. |
| [rows](/cells/python-net/aspose.cells/cells/rows) | Gets the collection of [Row](/cells/python-net/aspose.cells/row) objects that represents the individual rows in this worksheet. |
| [merged_cells](/cells/python-net/aspose.cells/cells/merged_cells) | Gets the collection of merged cells. |
| [multi_thread_reading](/cells/python-net/aspose.cells/cells/multi_thread_reading) | Gets or sets whether the cells data model should support Multi-Thread reading.<br/>Default value of this property is false. |
| [memory_setting](/cells/python-net/aspose.cells/cells/memory_setting) | Gets or sets the memory usage option for this cells. |
| [style](/cells/python-net/aspose.cells/cells/style) | Gets and sets the default style. |
| [standard_width_inch](/cells/python-net/aspose.cells/cells/standard_width_inch) | Gets or sets the default column width in the worksheet, in unit of inches. |
| [standard_width_pixels](/cells/python-net/aspose.cells/cells/standard_width_pixels) | Gets or sets the default column width in the worksheet, in unit of pixels. |
| [standard_width](/cells/python-net/aspose.cells/cells/standard_width) | Gets or sets the default column width in the worksheet, in unit of characters. |
| [standard_height](/cells/python-net/aspose.cells/cells/standard_height) | Gets or sets the default row height in this worksheet, in unit of points. |
| [standard_height_pixels](/cells/python-net/aspose.cells/cells/standard_height_pixels) | Gets or sets the default row height in this worksheet, in unit of pixels. |
| [standard_height_inch](/cells/python-net/aspose.cells/cells/standard_height_inch) | Gets or sets the default row height in this worksheet, in unit of inches. |
| [preserve_string](/cells/python-net/aspose.cells/cells/preserve_string) | Gets or sets a value indicating whether all worksheet values are preserved as strings. <br/>Default is false. |
| [min_row](/cells/python-net/aspose.cells/cells/min_row) | Minimum row index of cell which contains data or style. |
| [max_row](/cells/python-net/aspose.cells/cells/max_row) | Maximum row index of cell which contains data or style. |
| [min_column](/cells/python-net/aspose.cells/cells/min_column) | Minimum column index of those cells that have been instantiated in the collection(does not include the column<br/>where style is defined for the whole column but no cell has been instantiated in it). |
| [max_column](/cells/python-net/aspose.cells/cells/max_column) | Minimum column index of those cells that have been instantiated in the collection(does not include the column<br/>where style is defined for the whole column but no cell has been instantiated in it). |
| [min_data_row](/cells/python-net/aspose.cells/cells/min_data_row) | Minimum row index of cell which contains data. |
| [max_data_row](/cells/python-net/aspose.cells/cells/max_data_row) | Maximum row index of cell which contains data. |
| [min_data_column](/cells/python-net/aspose.cells/cells/min_data_column) | Minimum column index of cell which contains data. |
| [max_data_column](/cells/python-net/aspose.cells/cells/max_data_column) | Maximum column index of cell which contains data. |
| [is_default_row_height_matched](/cells/python-net/aspose.cells/cells/is_default_row_height_matched) | Indicates that row height and default font height matches |
| [is_default_row_hidden](/cells/python-net/aspose.cells/cells/is_default_row_hidden) | Indicates whether the row is default hidden. |
| [columns](/cells/python-net/aspose.cells/cells/columns) | Gets the collection of [Column](/cells/python-net/aspose.cells/column) objects that represents the individual columns in this worksheet. |
| [ranges](/cells/python-net/aspose.cells/cells/ranges) | Gets the collection of [Range](/cells/python-net/aspose.cells/range) objects created at run time. |
| [last_cell](/cells/python-net/aspose.cells/cells/last_cell) | Gets the last cell in this worksheet. |
| [max_display_range](/cells/python-net/aspose.cells/cells/max_display_range) | Gets the max range which includes data, merged cells and shapes. |
| [first_cell](/cells/python-net/aspose.cells/cells/first_cell) | Gets the first cell in this worksheet. |



Gets [Cell](/cells/python-net/aspose.cells/cell) item within the worksheet
### Indexer
| Name | Description |
| :- | :- |
| [index] | The zero based index of the element. |


### Methods
| Method | Description |
| :- | :- |
| [create_range(upper_left_cell, lower_right_cell)](/cells/python-net/aspose.cells/cells/create_range/#str-str) | Creates a [Range](/cells/python-net/aspose.cells/range) object from a range of cells. |
| [create_range(first_row, first_column, total_rows, total_columns)](/cells/python-net/aspose.cells/cells/create_range/#int-int-int-int) | Creates a [Range](/cells/python-net/aspose.cells/range) object from a range of cells. |
| [create_range(address)](/cells/python-net/aspose.cells/cells/create_range/#str) | Creates a [Range](/cells/python-net/aspose.cells/range) object from an address of the range. |
| [create_range(first_index, number, is_vertical)](/cells/python-net/aspose.cells/cells/create_range/#int-int-bool) | Creates a [Range](/cells/python-net/aspose.cells/range) object from rows of cells or columns of cells. |
| [get(row, column)](/cells/python-net/aspose.cells/cells/get/#int-int) | Add API for Python Via .Net.since this[int row, int column] is unsupported |
| [get(cell_name)](/cells/python-net/aspose.cells/cells/get/#str) | Add API for Python Via .Net.since this[string cellName] is unsupported |
| [import_object_array(obj_array, first_row, first_column, is_vertical)](/cells/python-net/aspose.cells/cells/import_object_array/#list-int-int-bool) | Imports an array of data into a worksheet. |
| [import_object_array(obj_array, first_row, first_column, is_vertical, skip)](/cells/python-net/aspose.cells/cells/import_object_array/#list-int-int-bool-int) | Imports an array of data into a worksheet. |
| [import_array(string_array, first_row, first_column, is_vertical)](/cells/python-net/aspose.cells/cells/import_array/#list-int-int-bool) | Imports an array of string into a worksheet. |
| [import_array(int_array, first_row, first_column, is_vertical)](/cells/python-net/aspose.cells/cells/import_array/#list-int-int-bool) | Imports an array of integer into a worksheet. |
| [import_array(double_array, first_row, first_column, is_vertical)](/cells/python-net/aspose.cells/cells/import_array/#list-int-int-bool) | Imports an array of double into a worksheet. |
| [import_csv(file_name, splitter, convert_numeric_data, first_row, first_column)](/cells/python-net/aspose.cells/cells/import_csv/#str-str-bool-int-int) | Import a CSV file to the cells. |
| [import_csv(stream, splitter, convert_numeric_data, first_row, first_column)](/cells/python-net/aspose.cells/cells/import_csv/#io.RawIOBase-str-bool-int-int) | Import a CSV file to the cells. |
| [import_csv(file_name, options, first_row, first_column)](/cells/python-net/aspose.cells/cells/import_csv/#str-TxtLoadOptions-int-int) | Import a CSV file to the cells. |
| [import_csv(stream, options, first_row, first_column)](/cells/python-net/aspose.cells/cells/import_csv/#io.RawIOBase-TxtLoadOptions-int-int) | Import a CSV file to the cells. |
| [merge(first_row, first_column, total_rows, total_columns)](/cells/python-net/aspose.cells/cells/merge/#int-int-int-int) | Merges a specified range of cells into a single cell. |
| [merge(first_row, first_column, total_rows, total_columns, merge_conflict)](/cells/python-net/aspose.cells/cells/merge/#int-int-int-int-bool) | Merges a specified range of cells into a single cell. |
| [merge(first_row, first_column, total_rows, total_columns, check_conflict, merge_conflict)](/cells/python-net/aspose.cells/cells/merge/#int-int-int-int-bool-bool) | Merges a specified range of cells into a single cell. |
| [copy_columns(source_cells0, source_column_index, destination_column_index, column_number, paste_options)](/cells/python-net/aspose.cells/cells/copy_columns/#Cells-int-int-int-PasteOptions) | Copies data and formats of a whole column. |
| [copy_columns(source_cells0, source_column_index, destination_column_index, column_number)](/cells/python-net/aspose.cells/cells/copy_columns/#Cells-int-int-int) | Copies data and formats of a whole column. |
| [copy_columns(source_cells, source_column_index, source_total_columns, destination_column_index, destination_total_columns)](/cells/python-net/aspose.cells/cells/copy_columns/#Cells-int-int-int-int) | Copies data and formats of the whole columns. |
| [copy_rows(source_cells, source_row_index, destination_row_index, row_number)](/cells/python-net/aspose.cells/cells/copy_rows/#Cells-int-int-int) | Copies data and formats of some whole rows. |
| [copy_rows(source_cells0, source_row_index, destination_row_index, row_number, copy_options)](/cells/python-net/aspose.cells/cells/copy_rows/#Cells-int-int-int-CopyOptions) | Copies data and formats of some whole rows. |
| [copy_rows(source_cells0, source_row_index, destination_row_index, row_number, copy_options, paste_options)](/cells/python-net/aspose.cells/cells/copy_rows/#Cells-int-int-int-CopyOptions-PasteOptions) | Copies data and formats of some whole rows. |
| [group_columns(first_index, last_index)](/cells/python-net/aspose.cells/cells/group_columns/#int-int) | Groups columns. |
| [group_columns(first_index, last_index, is_hidden)](/cells/python-net/aspose.cells/cells/group_columns/#int-int-bool) | Groups columns. |
| [ungroup_rows(first_index, last_index, is_all)](/cells/python-net/aspose.cells/cells/ungroup_rows/#int-int-bool) | Ungroups rows. |
| [ungroup_rows(first_index, last_index)](/cells/python-net/aspose.cells/cells/ungroup_rows/#int-int) | Ungroups rows. |
| [group_rows(first_index, last_index, is_hidden)](/cells/python-net/aspose.cells/cells/group_rows/#int-int-bool) | Groups rows. |
| [group_rows(first_index, last_index)](/cells/python-net/aspose.cells/cells/group_rows/#int-int) | Groups rows. |
| [delete_column(column_index, update_reference)](/cells/python-net/aspose.cells/cells/delete_column/#int-bool) | Deletes a column. |
| [delete_column(column_index)](/cells/python-net/aspose.cells/cells/delete_column/#int) | Deletes a column. |
| [delete_rows(row_index, total_rows)](/cells/python-net/aspose.cells/cells/delete_rows/#int-int) | Deletes several rows. |
| [delete_rows(row_index, total_rows, update_reference)](/cells/python-net/aspose.cells/cells/delete_rows/#int-int-bool) | Deletes multiple rows in the worksheet. |
| [delete_blank_columns()](/cells/python-net/aspose.cells/cells/delete_blank_columns/#) | Delete all blank columns which do not contain any data. |
| [delete_blank_columns(options)](/cells/python-net/aspose.cells/cells/delete_blank_columns/#DeleteOptions) | Delete all blank columns which do not contain any data. |
| [delete_blank_rows()](/cells/python-net/aspose.cells/cells/delete_blank_rows/#) | Delete all blank rows which do not contain any data. |
| [delete_blank_rows(options)](/cells/python-net/aspose.cells/cells/delete_blank_rows/#DeleteOptions) | Delete all blank rows which do not contain any data. |
| [insert_columns(column_index, total_columns)](/cells/python-net/aspose.cells/cells/insert_columns/#int-int) | Inserts some columns into the worksheet. |
| [insert_columns(column_index, total_columns, update_reference)](/cells/python-net/aspose.cells/cells/insert_columns/#int-int-bool) | Inserts some columns into the worksheet. |
| [insert_column(column_index, update_reference)](/cells/python-net/aspose.cells/cells/insert_column/#int-bool) | Inserts a new column into the worksheet. |
| [insert_column(column_index)](/cells/python-net/aspose.cells/cells/insert_column/#int) | Inserts a new column into the worksheet. |
| [insert_rows(row_index, total_rows, update_reference)](/cells/python-net/aspose.cells/cells/insert_rows/#int-int-bool) | Inserts multiple rows into the worksheet. |
| [insert_rows(row_index, total_rows, options)](/cells/python-net/aspose.cells/cells/insert_rows/#int-int-InsertOptions) | Inserts multiple rows into the worksheet. |
| [insert_rows(row_index, total_rows)](/cells/python-net/aspose.cells/cells/insert_rows/#int-int) | Inserts multiple rows into the worksheet. |
| [clear_range(range)](/cells/python-net/aspose.cells/cells/clear_range/#CellArea) | Clears contents and formatting of a range. |
| [clear_range(start_row, start_column, end_row, end_column)](/cells/python-net/aspose.cells/cells/clear_range/#int-int-int-int) | Clears contents and formatting of a range. |
| [clear_contents(range)](/cells/python-net/aspose.cells/cells/clear_contents/#CellArea) | Clears contents of a range. |
| [clear_contents(start_row, start_column, end_row, end_column)](/cells/python-net/aspose.cells/cells/clear_contents/#int-int-int-int) | Clears contents of a range. |
| [clear_formats(range)](/cells/python-net/aspose.cells/cells/clear_formats/#CellArea) | Clears formatting of a range. |
| [clear_formats(start_row, start_column, end_row, end_column)](/cells/python-net/aspose.cells/cells/clear_formats/#int-int-int-int) | Clears formatting of a range. |
| [find(what, previous_cell)](/cells/python-net/aspose.cells/cells/find/#any-Cell) | Finds the cell containing with the input object. |
| [find(what, previous_cell, find_options)](/cells/python-net/aspose.cells/cells/find/#any-Cell-FindOptions) | Finds the cell containing with the input object. |
| [end_cell_in_row(row_index)](/cells/python-net/aspose.cells/cells/end_cell_in_row/#int) | Gets the last cell in this row. |
| [end_cell_in_row(start_row, end_row, start_column, end_column)](/cells/python-net/aspose.cells/cells/end_cell_in_row/#int-int-int-int) | Gets the last cell with maximum row index in this range. |
| [end_cell_in_column(column_index)](/cells/python-net/aspose.cells/cells/end_cell_in_column/#int) | Gets the last cell in this column. |
| [end_cell_in_column(start_row, end_row, start_column, end_column)](/cells/python-net/aspose.cells/cells/end_cell_in_column/#int-int-int-int) | Gets the last cell with maximum column index in this range. |
| [insert_range(area, shift_number, shift_type, update_reference)](/cells/python-net/aspose.cells/cells/insert_range/#CellArea-int-ShiftType-bool) | Inserts a range of cells and shift cells according to the shift option. |
| [insert_range(area, shift_type)](/cells/python-net/aspose.cells/cells/insert_range/#CellArea-ShiftType) | Inserts a range of cells and shift cells according to the shift option. |
| [insert_range(area, shift_number, shift_type)](/cells/python-net/aspose.cells/cells/insert_range/#CellArea-int-ShiftType) | Inserts a range of cells and shift cells according to the shift option. |
| [import_custom_objects(list, property_names, is_property_name_shown, first_row, first_column, row_number, insert_rows, date_format_string, convert_string_to_number)](/cells/python-net/aspose.cells/cells/import_custom_objects/#list-list-bool-int-int-int-bool-str-bool) | Imports custom objects. |
| [import_custom_objects(list, first_row, first_column, options)](/cells/python-net/aspose.cells/cells/import_custom_objects/#list-int-int-ImportTableOptions) | Imports custom objects. |
| [subtotal(ca, group_by, function, total_list)](/cells/python-net/aspose.cells/cells/subtotal/#CellArea-int-ConsolidationFunction-list) | Creates subtotals for the range. |
| [subtotal(ca, group_by, function, total_list, replace, page_breaks, summary_below_data)](/cells/python-net/aspose.cells/cells/subtotal/#CellArea-int-ConsolidationFunction-list-bool-bool-bool) | Creates subtotals for the range. |
| [remove_duplicates()](/cells/python-net/aspose.cells/cells/remove_duplicates/#) | Removes duplicate rows in the sheet. |
| [remove_duplicates(start_row, start_column, end_row, end_column)](/cells/python-net/aspose.cells/cells/remove_duplicates/#int-int-int-int) | Removes duplicate values in the range. |
| [remove_duplicates(start_row, start_column, end_row, end_column, has_headers, column_offsets)](/cells/python-net/aspose.cells/cells/remove_duplicates/#int-int-int-int-bool-list) | Removes duplicate data of the range. |
| [get_row_enumerator()](/cells/python-net/aspose.cells/cells/get_row_enumerator/#) | Gets the rows enumerator. |
| [get_cell(row, column)](/cells/python-net/aspose.cells/cells/get_cell/#int-int) | Gets the [Cell](/cells/python-net/aspose.cells/cell) element or null at the specified cell row index and column index. |
| [get_row(row)](/cells/python-net/aspose.cells/cells/get_row/#int) | Gets the [Row](/cells/python-net/aspose.cells/row) element at the specified cell row index. |
| [check_cell(row, column)](/cells/python-net/aspose.cells/cells/check_cell/#int-int) | Gets the [Cell](/cells/python-net/aspose.cells/cell) element or null at the specified cell row index and column index. |
| [check_row(row)](/cells/python-net/aspose.cells/cells/check_row/#int) | Gets the [Row](/cells/python-net/aspose.cells/row) element or at the specified cell row index. |
| [check_column(column_index)](/cells/python-net/aspose.cells/cells/check_column/#int) | Gets the [Column](/cells/python-net/aspose.cells/column) element or null at the specified column index. |
| [is_row_hidden(row_index)](/cells/python-net/aspose.cells/cells/is_row_hidden/#int) | Checks whether a row at given index is hidden. |
| [is_column_hidden(column_index)](/cells/python-net/aspose.cells/cells/is_column_hidden/#int) | Checks whether a column at given index is hidden. |
| [add_range(range_object)](/cells/python-net/aspose.cells/cells/add_range/#Range) | Adds a range object reference to cells |
| [clear()](/cells/python-net/aspose.cells/cells/clear/#) | Clears all cell and row objects. |
| [import_data(table, first_row, first_column, options)](/cells/python-net/aspose.cells/cells/import_data/#ICellsDataTable-int-int-ImportTableOptions) | Import data from custom data table. |
| [import_array_list(array_list, first_row, first_column, is_vertical)](/cells/python-net/aspose.cells/cells/import_array_list/#list-int-int-bool) | Imports an arraylist of data into a worksheet. |
| [import_formula_array(string_array, first_row, first_column, is_vertical)](/cells/python-net/aspose.cells/cells/import_formula_array/#list-int-int-bool) | Imports an array of formula into a worksheet. |
| [text_to_columns(row, column, total_rows, options)](/cells/python-net/aspose.cells/cells/text_to_columns/#int-int-int-TxtLoadOptions) | Splits the text in the column to columns. |
| [un_merge(first_row, first_column, total_rows, total_columns)](/cells/python-net/aspose.cells/cells/un_merge/#int-int-int-int) | Unmerges a specified range of merged cells. |
| [clear_merged_cells()](/cells/python-net/aspose.cells/cells/clear_merged_cells/#) | Clears all merged ranges. |
| [hide_row(row)](/cells/python-net/aspose.cells/cells/hide_row/#int) | Hides a row. |
| [unhide_row(row, height)](/cells/python-net/aspose.cells/cells/unhide_row/#int-float) | Unhides a row. |
| [hide_rows(row, total_rows)](/cells/python-net/aspose.cells/cells/hide_rows/#int-int) | Hides multiple rows. |
| [unhide_rows(row, total_rows, height)](/cells/python-net/aspose.cells/cells/unhide_rows/#int-int-float) | Unhides the hidden rows. |
| [set_row_height_pixel(row, pixels)](/cells/python-net/aspose.cells/cells/set_row_height_pixel/#int-int) | Sets row height in unit of pixels. |
| [set_row_height_inch(row, inches)](/cells/python-net/aspose.cells/cells/set_row_height_inch/#int-float) | Sets row height in unit of inches. |
| [set_row_height(row, height)](/cells/python-net/aspose.cells/cells/set_row_height/#int-float) | Sets the height of the specified row. |
| [get_row_original_height_point(row)](/cells/python-net/aspose.cells/cells/get_row_original_height_point/#int) | Gets original row's height in unit of point if the row is hidden |
| [hide_column(column)](/cells/python-net/aspose.cells/cells/hide_column/#int) | Hides a column. |
| [unhide_column(column, width)](/cells/python-net/aspose.cells/cells/unhide_column/#int-float) | Unhides a column |
| [hide_columns(column, total_columns)](/cells/python-net/aspose.cells/cells/hide_columns/#int-int) | Hide multiple columns. |
| [unhide_columns(column, total_columns, width)](/cells/python-net/aspose.cells/cells/unhide_columns/#int-int-float) | Unhide multiple columns. |
| [get_row_height(row)](/cells/python-net/aspose.cells/cells/get_row_height/#int) | Gets the height of a specified row. |
| [get_view_row_height(row)](/cells/python-net/aspose.cells/cells/get_view_row_height/#int) | Gets the height of a specified row. |
| [get_row_height_pixel(row)](/cells/python-net/aspose.cells/cells/get_row_height_pixel/#int) | Gets the height of a specified row in unit of pixel. |
| [get_row_height_inch(row)](/cells/python-net/aspose.cells/cells/get_row_height_inch/#int) | Gets the height of a specified row in unit of inches. |
| [get_view_row_height_inch(row)](/cells/python-net/aspose.cells/cells/get_view_row_height_inch/#int) | Gets the height of a specified row in unit of inches. |
| [set_column_width_pixel(column, pixels)](/cells/python-net/aspose.cells/cells/set_column_width_pixel/#int-int) | Sets column width in unit of pixels in normal view. |
| [set_column_width_inch(column, inches)](/cells/python-net/aspose.cells/cells/set_column_width_inch/#int-float) | Sets column width in unit of inches  in normal view. |
| [set_column_width(column, width)](/cells/python-net/aspose.cells/cells/set_column_width/#int-float) | Sets the width of the specified column in normal view. |
| [get_column_width_pixel(column)](/cells/python-net/aspose.cells/cells/get_column_width_pixel/#int) | Gets the width of the specified column in normal view, in units of pixel. |
| [get_column_width_inch(column)](/cells/python-net/aspose.cells/cells/get_column_width_inch/#int) | Gets the width of the specified column in normal view, in units of inches. |
| [get_column_width(column)](/cells/python-net/aspose.cells/cells/get_column_width/#int) | Gets the width of the specified column in normal view |
| [get_view_column_width_pixel(column)](/cells/python-net/aspose.cells/cells/get_view_column_width_pixel/#int) | Get the width in different view type. |
| [set_view_column_width_pixel(column, pixels)](/cells/python-net/aspose.cells/cells/set_view_column_width_pixel/#int-int) | Sets the width of the column in different view. |
| [get_last_data_row(column)](/cells/python-net/aspose.cells/cells/get_last_data_row/#int) | Gets the last row index of cell which contains data in the specified column. |
| [apply_column_style(column, style, flag)](/cells/python-net/aspose.cells/cells/apply_column_style/#int-Style-StyleFlag) | Applies formats for a whole column. |
| [apply_row_style(row, style, flag)](/cells/python-net/aspose.cells/cells/apply_row_style/#int-Style-StyleFlag) | Applies formats for a whole row. |
| [apply_style(style, flag)](/cells/python-net/aspose.cells/cells/apply_style/#Style-StyleFlag) | Applies formats for a whole worksheet. |
| [copy_column(source_cells, source_column_index, destination_column_index)](/cells/python-net/aspose.cells/cells/copy_column/#Cells-int-int) | Copies data and formats of a whole column. |
| [copy_row(source_cells, source_row_index, destination_row_index)](/cells/python-net/aspose.cells/cells/copy_row/#Cells-int-int) | Copies data and formats of a whole row. |
| [get_grouped_row_outline_level(row_index)](/cells/python-net/aspose.cells/cells/get_grouped_row_outline_level/#int) | Gets the outline level (zero-based) of the row. |
| [get_grouped_column_outline_level(column_index)](/cells/python-net/aspose.cells/cells/get_grouped_column_outline_level/#int) | Gets the outline level (zero-based) of the column. |
| [get_max_grouped_column_outline_level()](/cells/python-net/aspose.cells/cells/get_max_grouped_column_outline_level/#) | Gets the max grouped column outline level (zero-based). |
| [get_max_grouped_row_outline_level()](/cells/python-net/aspose.cells/cells/get_max_grouped_row_outline_level/#) | Gets the max grouped row outline level (zero-based). |
| [show_group_detail(is_vertical, index)](/cells/python-net/aspose.cells/cells/show_group_detail/#bool-int) | Expands the grouped rows/columns. |
| [hide_group_detail(is_vertical, index)](/cells/python-net/aspose.cells/cells/hide_group_detail/#bool-int) | Collapses the grouped rows/columns. |
| [ungroup_columns(first_index, last_index)](/cells/python-net/aspose.cells/cells/ungroup_columns/#int-int) | Ungroups columns. |
| [delete_columns(column_index, total_columns, update_reference)](/cells/python-net/aspose.cells/cells/delete_columns/#int-int-bool) | Deletes several columns. |
| [is_deleting_range_enabled(start_row, start_column, total_rows, total_columns)](/cells/python-net/aspose.cells/cells/is_deleting_range_enabled/#int-int-int-int) | Check whether the range could be deleted. |
| [delete_row(row_index)](/cells/python-net/aspose.cells/cells/delete_row/#int) | Deletes a row. |
| [is_blank_column(column_index)](/cells/python-net/aspose.cells/cells/is_blank_column/#int) | Checks whether given column is blank(does not contain any data). |
| [insert_row(row_index)](/cells/python-net/aspose.cells/cells/insert_row/#int) | Inserts a new row into the worksheet. |
| [link_to_xml_map(map_name, row, column, path)](/cells/python-net/aspose.cells/cells/link_to_xml_map/#str-int-int-str) | Link to a xml map. |
| [find_formula(formula, previous_cell)](/cells/python-net/aspose.cells/cells/find_formula/#str-Cell) | Finds the cell with the input string. |
| [find_formula_contains(formula, previous_cell)](/cells/python-net/aspose.cells/cells/find_formula_contains/#str-Cell) | Finds the cell with formula which contains the input string. |
| [move_range(source_area, dest_row, dest_column)](/cells/python-net/aspose.cells/cells/move_range/#CellArea-int-int) | Moves the range. |
| [insert_cut_cells(cut_range, row, column, shift_type)](/cells/python-net/aspose.cells/cells/insert_cut_cells/#Range-int-int-ShiftType) | Insert cut range. |
| [delete_range(start_row, start_column, end_row, end_column, shift_type)](/cells/python-net/aspose.cells/cells/delete_range/#int-int-int-int-ShiftType) | Deletes a range of cells and shift cells according to the shift option. |
| [retrieve_subtotal_setting(ca)](/cells/python-net/aspose.cells/cells/retrieve_subtotal_setting/#CellArea) | Retrieves subtotals setting of the range. |
| [remove_formulas()](/cells/python-net/aspose.cells/cells/remove_formulas/#) | Removes all formula and replaces with the value of the formula. |
| [convert_string_to_numeric_value()](/cells/python-net/aspose.cells/cells/convert_string_to_numeric_value/#) | Converts string data in cells to numeric value if possible. |
| [get_dependents(is_all, row, column)](/cells/python-net/aspose.cells/cells/get_dependents/#bool-int-int) | Get all cells which refer to the specific cell. |
| [get_dependents_in_calculation(row, column, recursive)](/cells/python-net/aspose.cells/cells/get_dependents_in_calculation/#int-int-bool) | Gets all cells whose calculated result depends on specific cell. |
| [get_cell_style(row, column)](/cells/python-net/aspose.cells/cells/get_cell_style/#int-int) | Get the style of given cell. |


### See Also

* module [aspose.cells](../)
