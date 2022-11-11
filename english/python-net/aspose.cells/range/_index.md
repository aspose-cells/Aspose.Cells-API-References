---
title: Range
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 1250
url: /python-net/aspose.cells/range/
---

## Range class

Encapsulates the object that represents a range of cells within a spreadsheet.

The Range type exposes the following members:
## Properties
| Name | Description |
| :- | :- |
|current_region|Returns a Range object that represents the current region. <br/>            The current region is a range bounded by any combination of blank rows and blank columns.|
|hyperlinks|Gets all hyperlink in the range.|
|row_count|Gets the count of rows in the range.|
|column_count|Gets the count of columns in the range.|
|cell_count|Gets all cell count in the range.|
|name|Gets or sets the name of the range.|
|refers_to|Gets the range's refers to.|
|address|Gets address of the range.|
|left|Gets the distance, in points, from the left edge of column A to the left edge of the range.|
|top|Gets the distance, in points, from the top edge of row 1 to the top edge of the range.|
|width|Gets the width of a range in points.|
|height|Gets the width of a range in points.|
|first_row|Gets the index of the first row of the range.|
|first_column|Gets the index of the first column of the range.|
|value|Gets and sets the value of the range.|
|column_width|Sets or gets the column width of this range|
|row_height|Sets or gets the height of rows in this range|
|entire_column|Gets a Range object that represents the entire column (or columns) that contains the specified range.|
|entire_row|Gets a Range object that represents the entire row (or rows) that contains the specified range.|
|worksheet|Gets the [worksheet](/python-net/aspose.cells/range/)object which contains this range.|
## Methods
| Name | Description |
| :- | :- |
|auto_fill(target)|Automaticall fill the target range.|
|auto_fill(target, auto_fill_type)|Automaticall fill the target range.|
|set_outline_borders(border_style, border_color)|Sets the outline borders around a range of cells with same border style and color.|
|set_outline_borders(border_style, border_color)|Sets the outline borders around a range of cells with same border style and color.|
|set_outline_borders(border_styles, border_colors)|Sets out line borders around a range of cells.|
|set_outline_border(border_edge, border_style, border_color)|Sets the outline borders around a range of cells with same border style and color.|
|set_outline_border(border_edge, border_style, border_color)|Sets the outline borders around a range of cells with same border style and color.|
|copy(range, options)|Copying the range with paste special options.|
|copy(range)|Copies cell data (including formulas) from a source range.|
|get_enumerator()|Gets the enumerator for cells in this Range.|
|is_intersect(range)|Indicates whether the range is intersect.|
|intersect(range)|Returns a [Range](/python-net/aspose.cells/range/) object that represents the rectangular intersection of two ranges.|
|union(range)|Returns the union of two ranges.|
|merge()|Combines a range of cells into a single cell.|
|un_merge()|Unmerges merged cells of this range.|
|put_value(string_value, is_converted, set_style)|Puts a value into the range, if appropriate the value will be converted to other data type and cell's number format will be reset.|
|apply_style(style, flag)|Applies formats for a whole range.|
|set_style(style)|Sets the style of the range.|
|set_inside_borders(border_edge, line_style, border_color)|Set inside borders of the range.|
|move_to(dest_row, dest_column)|Move the current range to the dest range.|
|copy_data(range)|Copies cell data (including formulas) from a source range.|
|copy_value(range)|Copies cell value from a source range.|
|copy_style(range)|Copies style settings from a source range.|
|get_cell_or_null(row_offset, column_offset)|Gets [Cell](/python-net/aspose.cells/cell/) object or null in this range.|
|get_offset(row_offset, column_offset)|Gets [Range](/python-net/aspose.cells/range/) range by offset.|

### See Also

* namespace [aspose.cells](/python-net/aspose.cells/)
* assembly [Aspose.Cells](/python-net/)

