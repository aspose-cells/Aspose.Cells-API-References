---
title: AutoFilter
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 70
url: /python-net/aspose.cells/autofilter/
---

## AutoFilter class

Represents autofiltering for the specified worksheet.

The AutoFilter type exposes the following members:
## Properties
| Name | Description |
| :- | :- |
|sorter|Gets the data sorter.|
|range|Represents the range to which the specified AutoFilter applies.|
|show_filter_button|Indicates whether the AutoFilter button for this column is visible.|
|filter_columns|Gets the collection of the filter columns.|
## Methods
| Name | Description |
| :- | :- |
|remove_filter(field_index, criteria)|Removes a filter for a filter column.|
|remove_filter(field_index)|Removes a filter for a filter column.|
|custom(field_index, operator_type1, criteria1)|Filters a list with a custom criteria.|
|custom(field_index, operator_type1, criteria1, is_and, operator_type2, criteria2)|Filters a list with custom criteria.|
|refresh()|Refresh auto filters to hide or unhide the rows.|
|refresh(hide_rows)|Gets all hidden rows' indexes.|
|set_range(row, start_column, end_column)|Sets the range to which the specified AutoFilter applies.|
|get_cell_area()|Gets the [CellArea](/cells/python-net/aspose.cells/cellarea/) where the specified AutoFilter applies to.|
|add_filter(field_index, criteria)|Adds a filter for a filter column.|
|add_date_filter(field_index, date_time_grouping_type, year, month, day, hour, minute, second)|Adds a date filter.|
|remove_date_filter(field_index, date_time_grouping_type, year, month, day, hour, minute, second)|Removes a date filter.|
|filter(field_index, criteria)|Filters a list with specified criteria.|
|filter_top10(field_index, is_top, is_percent, item_count)|Filter the top 10 item in the list|
|dynamic_filter(field_index, dynamic_filter_type)|Adds a dynamic filter.|
|add_font_color_filter(field_index, color)|Adds a font color filter.|
|add_fill_color_filter(field_index, pattern, foreground_color, background_color)|Adds a fill color filter.|
|add_icon_filter(field_index, icon_set_type, icon_id)|Adds an icon filter.|
|match_blanks(field_index)|Match all blank cell in the list.|
|match_non_blanks(field_index)|Match all not blank cell in the list.|
|show_all()|Unhide all rows.|

### See Also

* namespace [aspose.cells](/cells/python-net/aspose.cells/)
* assembly [Aspose.Cells](/cells/python-net/)

