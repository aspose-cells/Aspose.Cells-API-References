---
title: Worksheet
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 1610
url: /cells/python-net/aspose.cells/worksheet/
---

## Worksheet class

Encapsulates the object that represents a single worksheet.

The Worksheet type exposes the following members:
## Properties
| Name | Description |
| :- | :- |
|protection|Represents the various types of protection options available for a worksheet. Supports advanced protection options in ExcelXP and above version.|
|unique_id|Gets and sets the unique id, it is same as {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}.|
|workbook|Gets the workbook object which contains this sheet.|
|cells|Gets the [cells](/cells/python-net/aspose.cells/worksheet/) collection.|
|query_tables|Gets [QueryTableCollection](/cells/python-net/aspose.cells/querytablecollection/) in the worksheet.|
|pivot_tables|Gets all pivot tables in this worksheet.|
|type|Represents worksheet type.|
|name|Gets or sets the name of the worksheet.|
|show_formulas|Indicates whether to show formulas or their results.|
|is_gridlines_visible|Gets or sets a value indicating whether the gridlines are visible.Default is true.|
|is_row_column_headers_visible|Gets or sets a value indicating whether the worksheet will display row and column headers.<br/>            Default is true.|
|pane_state|Indicates whether the pane has horizontal or vertical splits, and whether those splits are frozen.|
|display_zeros|True if zero values are displayed.|
|display_right_to_left|Indicates if the specified worksheet is displayed from right to left instead of from left to right.<br/>            Default is false.|
|is_outline_shown|Indicates whether to show outline.|
|is_selected|Indicates whether this worksheet is selected when the workbook is opened.|
|list_objects|Gets all ListObjects in this worksheet.|
|tab_id|Specifies the internal identifier for the sheet.|
|horizontal_page_breaks|Gets the [HorizontalPageBreakCollection](/cells/python-net/aspose.cells/horizontalpagebreakcollection/) collection.|
|vertical_page_breaks|Gets the [VerticalPageBreakCollection](/cells/python-net/aspose.cells/verticalpagebreakcollection/) collection.|
|hyperlinks|Gets the [HyperlinkCollection](/cells/python-net/aspose.cells/hyperlinkcollection/) collection.|
|page_setup|Represents the page setup description in this sheet.|
|auto_filter|Represents auto filter for the specified worksheet.|
|has_autofilter|Indicates whether this worksheet has auto filter.|
|transition_evaluation|Indicates whether the Transition Formula Evaluation (Lotus compatibility) option is enabled.|
|transition_entry|Indicates whether the Transition Formula Entry (Lotus compatibility) option is enabled.|
|visibility_type|Indicates the visible state for this sheet.|
|is_visible|Represents if the worksheet is visible.|
|sparkline_group_collection|Gets the sparkline group collection in the worksheet.|
|charts|Gets a [Chart](/cells/python-net/aspose.cells.charts/chart/) collection|
|comments|Gets the [Comment](/cells/python-net/aspose.cells/comment/) collection.|
|pictures|Gets a [Picture](/cells/python-net/aspose.cells.drawing/picture/) collection.|
|text_boxes|Gets a [TextBox](/cells/python-net/aspose.cells.drawing/textbox/) collection.|
|check_boxes|Gets a [CheckBox](/cells/python-net/aspose.cells.drawing/checkbox/) collection.|
|ole_objects|Represents a collection of [OleObject](/cells/python-net/aspose.cells.drawing/oleobject/) in a worksheet.|
|shapes|Returns all drawing shapes in this worksheet.|
|slicers|Get the Slicer collection in the worksheet|
|timelines|Get the Timeline collection in the worksheet|
|index|Gets the index of sheet in the worksheet collection.|
|is_protected|Indicates if the worksheet is protected.|
|validations|Gets the data validation setting collection in the worksheet.|
|allow_edit_ranges|Gets the allow edit range collection in the worksheet.|
|error_check_options|Gets error check setting applied on certain ranges.|
|outline|Gets the outline on this worksheet.|
|first_visible_row|Represents first visible row index.|
|first_visible_column|Represents first visible column index.|
|zoom|Represents the scaling factor in percentage. It should be between 10 and 400.|
|view_type|Gets and sets the view type.|
|is_page_break_preview|Indicates whether the specified worksheet is shown in normal view or page break preview.|
|is_ruler_visible|Indicates whether the ruler is visible. This property is only applied for page break preview.|
|tab_color|Represents worksheet tab color.|
|code_name|Gets worksheet code name.|
|background_image|Gets and sets worksheet background image.|
|conditional_formattings|Gets the ConditionalFormattings in the worksheet.|
|active_cell|Gets or sets the active cell in the worksheet.|
|custom_properties|Gets an object representing <br/>            the identifier information associated with a worksheet.|
|smart_tag_setting|Gets all [SmartTagCollection](/cells/python-net/aspose.cells.markup/smarttagcollection/) objects of the worksheet.|
|scenarios|Gets the collection of [Scenario](/cells/python-net/aspose.cells/scenario/).|
|cell_watches|Gets collection of cells on this worksheet being watched in the 'watch window'.|
## Methods
| Name | Description |
| :- | :- |
|freeze_panes(row, column, freezed_rows, freezed_columns)|Freezes panes at the specified cell in the worksheet.|
|freeze_panes(cell_name, freezed_rows, freezed_columns)|Freezes panes at the specified cell in the worksheet.|
|copy(source_sheet)|Copies contents and formats from another worksheet.|
|copy(source_sheet, copy_options)|Copies contents and formats from another worksheet.|
|auto_fit_column(column_index, first_row, last_row)|Autofits the column width.|
|auto_fit_column(column_index)|Autofits the column width.|
|auto_fit_columns()|Autofits all columns in this worksheet.|
|auto_fit_columns(options)|Autofits all columns in this worksheet.|
|auto_fit_columns(first_column, last_column)|Autofits the columns width.|
|auto_fit_columns(first_column, last_column, options)|Autofits the columns width.|
|auto_fit_columns(first_row, first_column, last_row, last_column)|Autofits the columns width.|
|auto_fit_columns(first_row, first_column, last_row, last_column, options)|Autofits the columns width.|
|auto_fit_row(row_index, first_column, last_column)|Autofits the row height.|
|auto_fit_row(row_index, first_column, last_column, options)|Autofits the row height.|
|auto_fit_row(start_row, end_row, start_column, end_column)|Autofits the row height.|
|auto_fit_row(row_index)|Autofits the row height.|
|auto_fit_rows()|Autofits all rows in this worksheet.|
|auto_fit_rows(only_auto)|Autofits all rows in this worksheet.|
|auto_fit_rows(options)|Autofits all rows in this worksheet.|
|auto_fit_rows(start_row, end_row)|Autofits row height in a range.|
|auto_fit_rows(start_row, end_row, options)|Autofits row height in a range.|
|protect(type)|Protects worksheet.|
|protect(type, password, old_password)|Protects worksheet.|
|unprotect()|Unprotects worksheet.|
|unprotect(password)|Unprotects worksheet.|
|calculate_formula(formula)|Calculates a formula.|
|calculate_formula(formula, opts)|Calculates a formula.|
|calculate_formula(recursive, ignore_error, custom_function)|Calculates all formulas in this worksheet.|
|calculate_formula(options, recursive)|Calculates all formulas in this worksheet.|
|get_panes()|Gets the window panes.|
|get_freezed_panes(row, column, freezed_rows, freezed_columns)|Gets the freeze panes.|
|split()|Splits window.|
|un_freeze_panes()|Unfreezes panes in the worksheet.|
|remove_split()|Removes split window.|
|add_page_breaks(cell_name)|Adds page break.|
|advanced_filter(is_filter, list_range, criteria_range, copy_to, unique_record_only)|Filters data using complex criteria.|
|remove_auto_filter()|Removes the auto filter of the worksheet.|
|set_visible(is_visible, ignore_error)|Sets the visible options.|
|select_range(start_row, start_column, total_rows, total_columns, remove_others)|Selects a range.|
|remove_all_drawing_objects()|Removes all drawing objects in this worksheet.|
|clear_comments()|Clears all comments in designer spreadsheet.|
|move_to(index)|Moves the sheet to another location in the spreadsheet.|
|replace(old_string, new_string)|Replaces all cells' text with a new string.|
|get_selected_ranges()|Gets selected ranges of cells in the designer spreadsheet.|
|set_background(picture_data)|Sets worksheet background image.|
|get_printing_page_breaks(options)|Gets automatic page breaks.|
|start_access_cache(opts)|Starts the session that uses caches to access the data in this worksheet.|
|close_access_cache(opts)|Closes the session that uses caches to access the data in this worksheet.|
|xml_map_query(path, xml_map)|Query cell areas that mapped/linked to the specific path of xml map.|
|refresh_pivot_tables()|Refreshes all the PivotTables in this Worksheet.|

### See Also

* namespace [aspose.cells](/cells/python-net/aspose.cells/)
* assembly [Aspose.Cells](/cells/python-net/)

