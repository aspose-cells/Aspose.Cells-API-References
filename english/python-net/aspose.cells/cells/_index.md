---
title: Cells
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 180
url: /cells/python-net/aspose.cells/cells/
---

## Cells class

Encapsulates a collection of cell relevant objects, such as [Cell](/cells/python-net/aspose.cells/cell/), [Row](/cells/python-net/aspose.cells/row/), ...etc.

The Cells type exposes the following members:
## Properties
| Name | Description |
| :- | :- |
|ods_cell_fields|Gets the list of fields of ods.|
|count|Gets the total count of instantiated Cell objects.|
|count_large|Gets the total count of instantiated Cell objects.|
|rows|Gets the collection of [Row](/cells/python-net/aspose.cells/row/) objects that represents the individual rows in this worksheet.|
|merged_cells|Gets the collection of merged cells.|
|multi_thread_reading|Gets or sets whether the cells data model should support Multi-Thread reading.<br/>            Default value of this property is false.|
|memory_setting|Gets or sets the memory usage option for this cells.|
|style|Gets and sets the default style.|
|standard_width_inch|Gets or sets the default column width in the worksheet, in unit of inches.|
|standard_width_pixels|Gets or sets the default column width in the worksheet, in unit of pixels.|
|standard_width|Gets or sets the default column width in the worksheet, in unit of characters.|
|standard_height|Gets or sets the default row height in this worksheet, in unit of points.|
|standard_height_pixels|Gets or sets the default row height in this worksheet, in unit of pixels.|
|standard_height_inch|Gets or sets the default row height in this worksheet, in unit of inches.|
|preserve_string|Gets or sets a value indicating whether all worksheet values are preserved as strings. <br/>            Default is false.|
|min_row|Minimum row index of cell which contains data or style.|
|max_row|Maximum row index of cell which contains data or style.|
|min_column|Minimum column index of those cells that have been instantiated in the collection(does not include the column<br/>            where style is defined for the whole column but no cell has been instantiated in it).|
|max_column|Minimum column index of those cells that have been instantiated in the collection(does not include the column<br/>            where style is defined for the whole column but no cell has been instantiated in it).|
|min_data_row|Minimum row index of cell which contains data.|
|max_data_row|Maximum row index of cell which contains data.|
|min_data_column|Minimum column index of cell which contains data.|
|max_data_column|Maximum column index of cell which contains data.|
|is_default_row_height_matched|Indicates that row height and default font height matches|
|is_default_row_hidden|Indicates whether the row is default hidden.|
|columns|Gets the collection of [Column](/cells/python-net/aspose.cells/column/) objects that represents the individual columns in this worksheet.|
|ranges|Gets the collection of [Range](/cells/python-net/aspose.cells/range/) objects created at run time.|
|last_cell|Gets the last cell in this worksheet.|
|max_display_range|Gets the max range which includes data, merged cells and shapes.|
|first_cell|Gets the first cell in this worksheet.|
## Indexer
| Name | Description |
| :- | :- |
|[index]|Gets [Cell](/cells/python-net/aspose.cells/cell/) item within the worksheet|
## Methods
| Name | Description |
| :- | :- |
|create_range(upper_left_cell, lower_right_cell)|Creates a [Range](/cells/python-net/aspose.cells/range/) object from a range of cells.|
|create_range(first_row, first_column, total_rows, total_columns)|Creates a [Range](/cells/python-net/aspose.cells/range/) object from a range of cells.|
|create_range(address)|Creates a [Range](/cells/python-net/aspose.cells/range/) object from a range of cells.|
|create_range(first_index, number, is_vertical)|Creates a [Range](/cells/python-net/aspose.cells/range/) object from rows of cells or columns of cells.|
|get(row, column)|Gets the [Cell](/cells/python-net/aspose.cells/cell/) element or null at the specified cell row index and column index.|
|get(cell_name)|Add API for Python Via .Net.since this[string cellName] is unsupported|
|import_object_array(obj_array, first_row, first_column, is_vertical)|Imports an array of data into a worksheet.|
|import_object_array(obj_array, first_row, first_column, is_vertical, skip)|Imports an array of data into a worksheet.|
|import_array(string_array, first_row, first_column, is_vertical)|Imports an array of string into a worksheet.|
|import_array(int_array, first_row, first_column, is_vertical)|Imports an array of integer into a worksheet.|
|import_array(double_array, first_row, first_column, is_vertical)|Imports an array of double into a worksheet.|
|import_csv(file_name, splitter, convert_numeric_data, first_row, first_column)|Import a CSV file to the cells.|
|import_csv(stream, splitter, convert_numeric_data, first_row, first_column)|Import a CSV file to the cells.|
|import_csv(file_name, options, first_row, first_column)|Import a CSV file to the cells.|
|import_csv(stream, options, first_row, first_column)|Import a CSV file to the cells.|
|merge(first_row, first_column, total_rows, total_columns)|Merges a specified range of cells into a single cell.|
|merge(first_row, first_column, total_rows, total_columns, merge_conflict)|Merges a specified range of cells into a single cell.|
|merge(first_row, first_column, total_rows, total_columns, check_conflict, merge_conflict)|Merges a specified range of cells into a single cell.|
|copy_columns(source_cells0, source_column_index, destination_column_index, column_number, paste_options)|Copies data and formats of a whole column.|
|copy_columns(source_cells0, source_column_index, destination_column_index, column_number)|Copies data and formats of a whole column.|
|copy_columns(source_cells, source_column_index, source_total_columns, destination_column_index, destination_total_columns)|Copies data and formats of a whole column.|
|copy_rows(source_cells, source_row_index, destination_row_index, row_number)|Copies data and formats of some whole rows.|
|copy_rows(source_cells0, source_row_index, destination_row_index, row_number, copy_options)|Copies data and formats of some whole rows.|
|copy_rows(source_cells0, source_row_index, destination_row_index, row_number, copy_options, paste_options)|Copies data and formats of some whole rows.|
|group_columns(first_index, last_index)|Groups columns.|
|group_columns(first_index, last_index, is_hidden)|Groups columns.|
|ungroup_rows(first_index, last_index, is_all)|Ungroups rows.|
|ungroup_rows(first_index, last_index)|Ungroups rows.|
|group_rows(first_index, last_index, is_hidden)|Groups rows.|
|group_rows(first_index, last_index)|Groups rows.|
|delete_column(column_index, update_reference)|Deletes a column.|
|delete_column(column_index)|Deletes a column.|
|delete_rows(row_index, total_rows)|Deletes several rows.|
|delete_rows(row_index, total_rows, update_reference)|Deletes multiple rows in the worksheet.|
|delete_blank_columns()|Delete all blank columns which do not contain any data.|
|delete_blank_columns(options)|Delete all blank columns which do not contain any data.|
|delete_blank_rows()|Delete all blank rows which do not contain any data.|
|delete_blank_rows(options)|Delete all blank rows which do not contain any data.|
|insert_columns(column_index, total_columns)|Inserts some columns into the worksheet.|
|insert_columns(column_index, total_columns, update_reference)|Inserts some columns into the worksheet.|
|insert_column(column_index, update_reference)|Inserts some columns into the worksheet.|
|insert_column(column_index)|Inserts some columns into the worksheet.|
|insert_rows(row_index, total_rows, update_reference)|Inserts multiple rows into the worksheet.|
|insert_rows(row_index, total_rows, options)|Inserts multiple rows into the worksheet.|
|insert_rows(row_index, total_rows)|Inserts multiple rows into the worksheet.|
|clear_range(range)|Clears contents and formatting of a range.|
|clear_range(start_row, start_column, end_row, end_column)|Clears contents and formatting of a range.|
|clear_contents(range)|Clears contents of a range.|
|clear_contents(start_row, start_column, end_row, end_column)|Clears contents of a range.|
|clear_formats(range)|Clears formatting of a range.|
|clear_formats(start_row, start_column, end_row, end_column)|Clears formatting of a range.|
|find(what, previous_cell)|Finds the cell containing with the input object.|
|find(what, previous_cell, find_options)|Finds the cell containing with the input object.|
|end_cell_in_row(row_index)|Gets the last cell in this row.|
|end_cell_in_row(start_row, end_row, start_column, end_column)|Gets the last cell in this row.|
|end_cell_in_column(column_index)|  |
|end_cell_in_column(start_row, end_row, start_column, end_column)|  |
|insert_range(area, shift_number, shift_type, update_reference)|Inserts a range of cells and shift cells according to the shift option.|
|insert_range(area, shift_type)|Inserts a range of cells and shift cells according to the shift option.|
|insert_range(area, shift_number, shift_type)|Inserts a range of cells and shift cells according to the shift option.|
|import_custom_objects(list, property_names, is_property_name_shown, first_row, first_column, row_number, insert_rows, date_format_string, convert_string_to_number)|Imports custom objects.|
|import_custom_objects(list, first_row, first_column, options)|Imports custom objects.|
|subtotal(ca, group_by, function, total_list)|Creates subtotals for the range.|
|subtotal(ca, group_by, function, total_list, replace, page_breaks, summary_below_data)|Creates subtotals for the range.|
|remove_duplicates()|Removes duplicate rows in the sheet.|
|remove_duplicates(start_row, start_column, end_row, end_column)|Removes duplicate values in the range.|
|remove_duplicates(start_row, start_column, end_row, end_column, has_headers, column_offsets)|Removes duplicate data of the range.|
|get_row_enumerator()|Gets the rows enumerator.|
|get_cell(row, column)|Gets the [Cell](/cells/python-net/aspose.cells/cell/) element or null at the specified cell row index and column index.|
|get_row(row)|Gets the [Row](/cells/python-net/aspose.cells/row/) element at the specified cell row index.|
|check_cell(row, column)|Gets the [Cell](/cells/python-net/aspose.cells/cell/) element or null at the specified cell row index and column index.|
|check_row(row)|Gets the [Row](/cells/python-net/aspose.cells/row/) element or at the specified cell row index.|
|check_column(column_index)|Gets the [Column](/cells/python-net/aspose.cells/column/) element or null at the specified column index.|
|is_row_hidden(row_index)|Checks whether a row at given index is hidden.|
|is_column_hidden(column_index)|Checks whether a column at given index is hidden.|
|add_range(range_object)|Adds a range object reference to cells|
|clear()|Clears all cell and row objects.|
|import_data(table, first_row, first_column, options)|Import data from custom data table.|
|import_array_list(array_list, first_row, first_column, is_vertical)|Imports an arraylist of data into a worksheet.|
|import_formula_array(string_array, first_row, first_column, is_vertical)|Imports an array of formula into a worksheet.|
|text_to_columns(row, column, total_rows, options)|Splits the text in the column to columns.|
|un_merge(first_row, first_column, total_rows, total_columns)|Unmerges a specified range of merged cells.|
|clear_merged_cells()|Clears all merged ranges.|
|hide_row(row)|Hides a row.|
|unhide_row(row, height)|Unhides a row.|
|hide_rows(row, total_rows)|Hides multiple rows.|
|unhide_rows(row, total_rows, height)|Unhides the hidden rows.|
|set_row_height_pixel(row, pixels)|Sets row height in unit of pixels.|
|set_row_height_inch(row, inches)|Sets row height in unit of inches.|
|set_row_height(row, height)|Sets row height in unit of inches.|
|get_row_original_height_point(row)|Gets original row's height in unit of point if the row is hidden|
|hide_column(column)|Hides a column.|
|unhide_column(column, width)|Unhides a column|
|hide_columns(column, total_columns)|Hide multiple columns.|
|unhide_columns(column, total_columns, width)|Unhide multiple columns.|
|get_row_height(row)|Gets the height of a specified row.|
|get_view_row_height(row)|Gets the height of a specified row.|
|get_row_height_pixel(row)|Gets the height of a specified row in unit of pixel.|
|get_row_height_inch(row)|Gets the height of a specified row in unit of inches.|
|get_view_row_height_inch(row)|Gets the height of a specified row in unit of inches.|
|set_column_width_pixel(column, pixels)|Sets column width in unit of pixels in normal view.|
|set_column_width_inch(column, inches)|Sets column width in unit of inches  in normal view.|
|set_column_width(column, width)|Sets column width in unit of inches  in normal view.|
|get_column_width_pixel(column)|Gets the width of the specified column in normal view, in units of pixel.|
|get_column_width_inch(column)|Gets the width of the specified column in normal view, in units of inches.|
|get_column_width(column)|Gets the width of the specified column in normal view, in units of pixel.|
|get_view_column_width_pixel(column)|Get the width in different view type.|
|set_view_column_width_pixel(column, pixels)|Sets the width of the column in different view.|
|get_last_data_row(column)|Gets the last row index of cell which contains data in the specified column.|
|apply_column_style(column, style, flag)|Applies formats for a whole column.|
|apply_row_style(row, style, flag)|Applies formats for a whole row.|
|apply_style(style, flag)|Applies formats for a whole worksheet.|
|copy_column(source_cells, source_column_index, destination_column_index)|Copies data and formats of a whole column.|
|copy_row(source_cells, source_row_index, destination_row_index)|Copies data and formats of a whole row.|
|get_grouped_row_outline_level(row_index)|Gets the outline level (zero-based) of the row.|
|get_grouped_column_outline_level(column_index)|Gets the outline level (zero-based) of the column.|
|get_max_grouped_column_outline_level()|Gets the max grouped column outline level (zero-based).|
|get_max_grouped_row_outline_level()|Gets the max grouped row outline level (zero-based).|
|show_group_detail(is_vertical, index)|Expands the grouped rows/columns.|
|hide_group_detail(is_vertical, index)|Collapses the grouped rows/columns.|
|ungroup_columns(first_index, last_index)|Ungroups columns.|
|delete_columns(column_index, total_columns, update_reference)|Deletes several columns.|
|is_deleting_range_enabled(start_row, start_column, total_rows, total_columns)|Check whether the range could be deleted.|
|delete_row(row_index)|Deletes several rows.|
|is_blank_column(column_index)|Checks whether given column is blank(does not contain any data).|
|insert_row(row_index)|Inserts multiple rows into the worksheet.|
|link_to_xml_map(map_name, row, column, path)|Link to a xml map.|
|find_formula(formula, previous_cell)|Finds the cell with the input string.|
|find_formula_contains(formula, previous_cell)|Finds the cell with formula which contains the input string.|
|move_range(source_area, dest_row, dest_column)|Moves the range.|
|insert_cut_cells(cut_range, row, column, shift_type)|Insert cut range.|
|delete_range(start_row, start_column, end_row, end_column, shift_type)|Deletes a range of cells and shift cells according to the shift option.|
|retrieve_subtotal_setting(ca)|Retrieves subtotals setting of the range.|
|remove_formulas()|Removes all formula and replaces with the value of the formula.|
|convert_string_to_numeric_value()|Converts string data in cells to numeric value if possible.|
|get_dependents(is_all, row, column)|Get all cells which refer to the specific cell.|
|get_dependents_in_calculation(row, column, recursive)|Gets all cells whose calculated result depends on specific cell.|
|get_cell_style(row, column)|Get the style of given cell.|

### See Also

* namespace [aspose.cells](/cells/python-net/aspose.cells/)
* assembly [Aspose.Cells](/cells/python-net/)

