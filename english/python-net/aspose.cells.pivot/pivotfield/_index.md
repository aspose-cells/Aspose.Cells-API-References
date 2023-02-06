---
title: PivotField class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 10
url: /python-net/aspose.cells.pivot/pivotfield/
is_root: false
---

## PivotField class

Represents a field in a PivotTable report.



The PivotField type exposes the following members:

### Properties
| Property | Description |
| :- | :- |
| [pivot_items](/cells/python-net/aspose.cells.pivot/pivotfield/pivot_items) | Gets the pivot items of the pivot field |
| [range](/cells/python-net/aspose.cells.pivot/pivotfield/range) | Gets the group range of the pivot field |
| [is_calculated_field](/cells/python-net/aspose.cells.pivot/pivotfield/is_calculated_field) | Indicates whether the specified PivotTable field is calculated field. |
| [base_index](/cells/python-net/aspose.cells.pivot/pivotfield/base_index) | Represents the PivotField index in the base PivotFields. |
| [position](/cells/python-net/aspose.cells.pivot/pivotfield/position) | Represents the PivotField index in the PivotFields. |
| [name](/cells/python-net/aspose.cells.pivot/pivotfield/name) | Represents the PivotField name. |
| [display_name](/cells/python-net/aspose.cells.pivot/pivotfield/display_name) | Represents the PivotField display name. |
| [is_auto_subtotals](/cells/python-net/aspose.cells.pivot/pivotfield/is_auto_subtotals) | Indicates whether the specified field shows automatic subtotals. Default is true. |
| [drag_to_column](/cells/python-net/aspose.cells.pivot/pivotfield/drag_to_column) | Indicates whether the specified field can be dragged to the column position.<br/>The default value is true. |
| [drag_to_hide](/cells/python-net/aspose.cells.pivot/pivotfield/drag_to_hide) | Indicates whether the specified field can be dragged to the hide position.<br/>The default value is true. |
| [drag_to_row](/cells/python-net/aspose.cells.pivot/pivotfield/drag_to_row) | Indicates whether the specified field can be dragged to the row position.<br/>The default value is true. |
| [drag_to_page](/cells/python-net/aspose.cells.pivot/pivotfield/drag_to_page) | Indicates whether the specified field can be dragged to the page position.<br/>The default value is true. |
| [drag_to_data](/cells/python-net/aspose.cells.pivot/pivotfield/drag_to_data) | Indicates whether the specified field can be dragged to the data position.<br/>The default value is true. |
| [is_multiple_item_selection_allowed](/cells/python-net/aspose.cells.pivot/pivotfield/is_multiple_item_selection_allowed) | indicates whether the field can have multiple items<br/>selected in the page field<br/>The default value is false. |
| [is_repeat_item_labels](/cells/python-net/aspose.cells.pivot/pivotfield/is_repeat_item_labels) | indicates whether the field can repeat items labels<br/>The default value is false. |
| [is_include_new_items_in_filter](/cells/python-net/aspose.cells.pivot/pivotfield/is_include_new_items_in_filter) | indicates whether the field can include new items in manual filter<br/>The default value is false. |
| [is_insert_page_breaks_between_items](/cells/python-net/aspose.cells.pivot/pivotfield/is_insert_page_breaks_between_items) | indicates whether the field can insert page breaks between items<br/>insert page break after each item<br/>The default value is false. |
| [show_all_items](/cells/python-net/aspose.cells.pivot/pivotfield/show_all_items) | Indicates whether all items in the PivotTable report are displayed, <br/>even if they don't contain summary data.<br/>show items with no data<br/>The default value is false. |
| [non_auto_sort_default](/cells/python-net/aspose.cells.pivot/pivotfield/non_auto_sort_default) | Indicates whether a sort operation that will be applied to this pivot field is an autosort operation or a simple data sort. |
| [is_auto_sort](/cells/python-net/aspose.cells.pivot/pivotfield/is_auto_sort) | Indicates whether the specified PivotTable field is automatically sorted. |
| [is_ascend_sort](/cells/python-net/aspose.cells.pivot/pivotfield/is_ascend_sort) | Indicates whether the specified PivotTable field is autosorted ascending. |
| [auto_sort_field](/cells/python-net/aspose.cells.pivot/pivotfield/auto_sort_field) | Represents auto sort field index. <br/>-1 means PivotField itself,others means the position of the data fields. |
| [is_auto_show](/cells/python-net/aspose.cells.pivot/pivotfield/is_auto_show) | Indicates whether the specified PivotTable field is automatically shown,only valid for excel 2003. |
| [is_ascend_show](/cells/python-net/aspose.cells.pivot/pivotfield/is_ascend_show) | Indicates whether the specified PivotTable field is autoshown ascending. |
| [auto_show_count](/cells/python-net/aspose.cells.pivot/pivotfield/auto_show_count) | Represent the number of top or bottom items<br/>that are automatically shown in the specified PivotTable field. |
| [auto_show_field](/cells/python-net/aspose.cells.pivot/pivotfield/auto_show_field) | Represents auto show field index. -1 means PivotField itself.<br/>It should be the index of the data fields. |
| [function](/cells/python-net/aspose.cells.pivot/pivotfield/function) | Represents the function used to summarize the PivotTable data field. |
| [data_display_format](/cells/python-net/aspose.cells.pivot/pivotfield/data_display_format) | Represents how to display the values contained in a data field. |
| [base_field_index](/cells/python-net/aspose.cells.pivot/pivotfield/base_field_index) | Represents the base field for a custom calculation. |
| [base_item_position](/cells/python-net/aspose.cells.pivot/pivotfield/base_item_position) | Represents the item in the base field for a custom calculation.<br/>Valid only for data fields. <br/>Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom,<br/>please set PivotField.BaseItemIndex attribute. |
| [base_item_index](/cells/python-net/aspose.cells.pivot/pivotfield/base_item_index) | Represents the item in the base field for a custom calculation.<br/>Valid only for data fields. |
| [current_page_item](/cells/python-net/aspose.cells.pivot/pivotfield/current_page_item) | Represents the current page item showing for the page field (valid only for page fields). |
| [number](/cells/python-net/aspose.cells.pivot/pivotfield/number) | Represents the built-in display format of numbers and dates. |
| [insert_blank_row](/cells/python-net/aspose.cells.pivot/pivotfield/insert_blank_row) | Indicates whether inserting blank line after each item. |
| [show_subtotal_at_top](/cells/python-net/aspose.cells.pivot/pivotfield/show_subtotal_at_top) | when ShowInOutlineForm is true, then display subtotals at the top of the list of items instead of at the bottom |
| [show_in_outline_form](/cells/python-net/aspose.cells.pivot/pivotfield/show_in_outline_form) | Indicates whether layout this field in outline form on the Pivot Table view |
| [number_format](/cells/python-net/aspose.cells.pivot/pivotfield/number_format) | Represents the custom display format of numbers and dates. |
| [items](/cells/python-net/aspose.cells.pivot/pivotfield/items) | Get all base items; |
| [original_items](/cells/python-net/aspose.cells.pivot/pivotfield/original_items) | Get the original base items; |
| [item_count](/cells/python-net/aspose.cells.pivot/pivotfield/item_count) | Gets the base item count of this pivot field. |
| [show_compact](/cells/python-net/aspose.cells.pivot/pivotfield/show_compact) | Indicates whether display labels from the next field in the same column on the Pivot Table view |


### Methods
| Method | Description |
| :- | :- |
| [hide_item(index, is_hidden)](/cells/python-net/aspose.cells.pivot/pivotfield/hide_item/#int-bool) | Sets whether the specific PivotItem in a data field is hidden. |
| [hide_item(item_value, is_hidden)](/cells/python-net/aspose.cells.pivot/pivotfield/hide_item/#str-bool) | Sets whether the specific PivotItem in a data field is hidden. |
| [get_pivot_filter_by_type(type)](/cells/python-net/aspose.cells.pivot/pivotfield/get_pivot_filter_by_type/#PivotFilterType) | Gets the pivot filter of the pivot field by type |
| [get_pivot_filters()](/cells/python-net/aspose.cells.pivot/pivotfield/get_pivot_filters/#) | Gets the pivot filters of the pivot field |
| [init_pivot_items()](/cells/python-net/aspose.cells.pivot/pivotfield/init_pivot_items/#) | Init the pivot items of the pivot field |
| [get_calculated_field_formula()](/cells/python-net/aspose.cells.pivot/pivotfield/get_calculated_field_formula/#) | Get the formula string of the specified calculated field . |
| [set_subtotals(subtotal_type, shown)](/cells/python-net/aspose.cells.pivot/pivotfield/set_subtotals/#PivotFieldSubtotalType-bool) | Sets whether the specified field shows that subtotals. |
| [get_subtotals(subtotal_type)](/cells/python-net/aspose.cells.pivot/pivotfield/get_subtotals/#PivotFieldSubtotalType) | Gets whether the specified field shows that subtotals. |
| [is_hidden_item(index)](/cells/python-net/aspose.cells.pivot/pivotfield/is_hidden_item/#int) | Indicates whether the specific PivotItem is hidden. |
| [is_hidden_item_detail(index)](/cells/python-net/aspose.cells.pivot/pivotfield/is_hidden_item_detail/#int) | Indicates whether the specific PivotItem is hidden detail. |
| [hide_item_detail(index, is_hidden_detail)](/cells/python-net/aspose.cells.pivot/pivotfield/hide_item_detail/#int-bool) | Sets whether the specific PivotItem in a pivot field is hidden detail. |
| [hide_detail(is_hidden_detail)](/cells/python-net/aspose.cells.pivot/pivotfield/hide_detail/#bool) | Sets whether the PivotItems in a pivot field is hidden detail.That is collapse/expand this field. |
| [add_calculated_item(name, formula)](/cells/python-net/aspose.cells.pivot/pivotfield/add_calculated_item/#str-str) | Add a calculated item to the pivot field. |



### Example 


```python
from aspose.cells import Workbook
from aspose.cells.pivot import PivotFieldType, PivotTableStyleType

book = Workbook()
sheet = book.worksheets[0]
cells = sheet.cells
cells.get(0, 0).value = "fruit"
cells.get(1, 0).value = "grape"
cells.get(2, 0).value = "blueberry"
cells.get(3, 0).value = "kiwi"
cells.get(4, 0).value = "cherry"
cells.get(5, 0).value = "grape"
cells.get(6, 0).value = "blueberry"
cells.get(7, 0).value = "kiwi"
cells.get(8, 0).value = "cherry"
cells.get(0, 1).value = "year"
cells.get(1, 1).value = 2020
cells.get(2, 1).value = 2020
cells.get(3, 1).value = 2020
cells.get(4, 1).value = 2020
cells.get(5, 1).value = 2021
cells.get(6, 1).value = 2021
cells.get(7, 1).value = 2021
cells.get(8, 1).value = 2021
cells.get(0, 2).value = "amount"
cells.get(1, 2).value = 50
cells.get(2, 2).value = 60
cells.get(3, 2).value = 70
cells.get(4, 2).value = 80
cells.get(5, 2).value = 90
cells.get(6, 2).value = 100
cells.get(7, 2).value = 110
cells.get(8, 2).value = 120
pivots = sheet.pivot_tables
pivotIndex = pivots.add("=Sheet1!A1:C9", "A12", "TestPivotTable")
pivot = pivots[pivotIndex]
pivot.add_field_to_area(PivotFieldType.ROW, "fruit")
pivot.add_field_to_area(PivotFieldType.COLUMN, "year")
pivot.add_field_to_area(PivotFieldType.DATA, "amount")
pivot.pivot_table_style_type = PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM10
# Change PivotField's attributes
rowField = pivot.row_fields[0]
rowField.display_name = "custom display name"
pivot.refresh_data()
pivot.calculate_data()
# do your business
book.save("out.xlsx")

```

### See Also
* module [aspose.cells.pivot](..)
