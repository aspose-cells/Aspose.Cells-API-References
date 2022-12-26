---
title: AutoFilter class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 70
url: /python-net/aspose.cells/autofilter/
is_root: false
---

## AutoFilter class

Represents autofiltering for the specified worksheet.



The AutoFilter type exposes the following members:

### Properties
| Property | Description |
| :- | :- |
| [sorter](/cells/python-net/aspose.cells/autofilter/sorter) | Gets the data sorter. |
| [range](/cells/python-net/aspose.cells/autofilter/range) | Represents the range to which the specified AutoFilter applies. |
| [show_filter_button](/cells/python-net/aspose.cells/autofilter/show_filter_button) | Indicates whether the AutoFilter button for this column is visible. |
| [filter_columns](/cells/python-net/aspose.cells/autofilter/filter_columns) | Gets the collection of the filter columns. |


### Methods
| Method | Description |
| :- | :- |
| [remove_filter(field_index, criteria)](/cells/python-net/aspose.cells/autofilter/remove_filter/#int-str) | Removes a filter for a filter column. |
| [remove_filter(field_index)](/cells/python-net/aspose.cells/autofilter/remove_filter/#int) | Remove the specific filter. |
| [custom(field_index, operator_type1, criteria1)](/cells/python-net/aspose.cells/autofilter/custom/#int-FilterOperatorType-any) | Filters a list with a custom criteria. |
| [custom(field_index, operator_type1, criteria1, is_and, operator_type2, criteria2)](/cells/python-net/aspose.cells/autofilter/custom/#int-FilterOperatorType-any-bool-FilterOperatorType-any) | Filters a list with custom criteria. |
| [refresh()](/cells/python-net/aspose.cells/autofilter/refresh/#) | Refresh auto filters to hide or unhide the rows. |
| [refresh(hide_rows)](/cells/python-net/aspose.cells/autofilter/refresh/#bool) | Gets all hidden rows' indexes. |
| [set_range(row, start_column, end_column)](/cells/python-net/aspose.cells/autofilter/set_range/#int-int-int) | Sets the range to which the specified AutoFilter applies. |
| [get_cell_area()](/cells/python-net/aspose.cells/autofilter/get_cell_area/#) | Gets the [CellArea](/cells/python-net/aspose.cells/cellarea) where the specified AutoFilter applies to. |
| [add_filter(field_index, criteria)](/cells/python-net/aspose.cells/autofilter/add_filter/#int-str) | Adds a filter for a filter column. |
| [add_date_filter(field_index, date_time_grouping_type, year, month, day, hour, minute, second)](/cells/python-net/aspose.cells/autofilter/add_date_filter/#int-DateTimeGroupingType-int-int-int-int-int-int) | Adds a date filter. |
| [remove_date_filter(field_index, date_time_grouping_type, year, month, day, hour, minute, second)](/cells/python-net/aspose.cells/autofilter/remove_date_filter/#int-DateTimeGroupingType-int-int-int-int-int-int) | Removes a date filter. |
| [filter(field_index, criteria)](/cells/python-net/aspose.cells/autofilter/filter/#int-str) | Filters a list with specified criteria. |
| [filter_top10(field_index, is_top, is_percent, item_count)](/cells/python-net/aspose.cells/autofilter/filter_top10/#int-bool-bool-int) | Filter the top 10 item in the list |
| [dynamic_filter(field_index, dynamic_filter_type)](/cells/python-net/aspose.cells/autofilter/dynamic_filter/#int-DynamicFilterType) | Adds a dynamic filter. |
| [add_font_color_filter(field_index, color)](/cells/python-net/aspose.cells/autofilter/add_font_color_filter/#int-CellsColor) | Adds a font color filter. |
| [add_fill_color_filter(field_index, pattern, foreground_color, background_color)](/cells/python-net/aspose.cells/autofilter/add_fill_color_filter/#int-BackgroundType-CellsColor-CellsColor) | Adds a fill color filter. |
| [add_icon_filter(field_index, icon_set_type, icon_id)](/cells/python-net/aspose.cells/autofilter/add_icon_filter/#int-IconSetType-int) | Adds an icon filter. |
| [match_blanks(field_index)](/cells/python-net/aspose.cells/autofilter/match_blanks/#int) | Match all blank cell in the list. |
| [match_non_blanks(field_index)](/cells/python-net/aspose.cells/autofilter/match_non_blanks/#int) | Match all not blank cell in the list. |
| [show_all()](/cells/python-net/aspose.cells/autofilter/show_all/#) | Unhide all rows. |


### See Also

* module [aspose.cells](../)
