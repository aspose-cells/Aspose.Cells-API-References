---
title: PivotField
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 10
url: /python-net/aspose.cells.pivot/pivotfield/
---

## PivotField class

Represents a field in a PivotTable report.

The PivotField type exposes the following members:
## Properties
| Name | Description |
| :- | :- |
|pivot_items|Gets the pivot items of the pivot field|
|range|Gets the group range of the pivot field|
|is_calculated_field|Indicates whether the specified PivotTable field is calculated field.|
|base_index|Represents the PivotField index in the base PivotFields.|
|position|Represents the PivotField index in the PivotFields.|
|name|Represents the PivotField name.|
|display_name|Represents the PivotField display name.|
|is_auto_subtotals|Indicates whether the specified field shows automatic subtotals. Default is true.|
|drag_to_column|Indicates whether the specified field can be dragged to the column position.<br/>            The default value is true.|
|drag_to_hide|Indicates whether the specified field can be dragged to the hide position.<br/>             The default value is true.|
|drag_to_row|Indicates whether the specified field can be dragged to the row position.<br/>            The default value is true.|
|drag_to_page|Indicates whether the specified field can be dragged to the page position.<br/>             The default value is true.|
|drag_to_data|Indicates whether the specified field can be dragged to the data position.<br/>             The default value is true.|
|is_multiple_item_selection_allowed|indicates whether the field can have multiple items<br/>            selected in the page field<br/>            The default value is false.|
|is_repeat_item_labels|indicates whether the field can repeat items labels<br/>            The default value is false.|
|is_include_new_items_in_filter|indicates whether the field can include new items in manual filter<br/>            The default value is false.|
|is_insert_page_breaks_between_items|indicates whether the field can insert page breaks between items<br/>            insert page break after each item<br/>            The default value is false.|
|show_all_items|Indicates whether all items in the PivotTable report are displayed, <br/>            even if they don't contain summary data.<br/>            show items with no data<br/>            The default value is false.|
|is_auto_sort|Indicates whether the specified PivotTable field is automatically sorted.|
|is_ascend_sort|Indicates whether the specified PivotTable field is autosorted ascending.|
|auto_sort_field|Represents auto sort field index. <br/>            -1 means PivotField itself,others means the position of the data fields.|
|is_auto_show|Indicates whether the specified PivotTable field is automatically shown,only valid for excel 2003.|
|is_ascend_show|Indicates whether the specified PivotTable field is autoshown ascending.|
|auto_show_count|Represent the number of top or bottom items<br/>            that are automatically shown in the specified PivotTable field.|
|auto_show_field|Represents auto show field index. -1 means PivotField itself.<br/>            It should be the index of the data fields.|
|function|Represents the function used to summarize the PivotTable data field.|
|data_display_format|Represents how to display the values contained in a data field.|
|base_field_index|Represents the base field for a custom calculation.|
|base_item_position|Represents the item in the base field for a custom calculation.<br/>             Valid only for data fields. <br/>             Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom,<br/>             please set PivotField.BaseItemIndex attribute.|
|base_item_index|Represents the item in the base field for a custom calculation.<br/>             Valid only for data fields.|
|current_page_item|Represents the current page item showing for the page field (valid only for page fields).|
|number|Represents the built-in display format of numbers and dates.|
|insert_blank_row|Indicates whether inserting blank line after each item.|
|show_subtotal_at_top|when ShowInOutlineForm is true, then display subtotals at the top of the list of items instead of at the bottom|
|show_in_outline_form|Indicates whether layout this field in outline form on the Pivot Table view|
|number_format|Represents the custom display format of numbers and dates.|
|items|Get all base items;|
|original_items|Get the original base items;|
|item_count|Gets the base item count of this pivot field.|
|show_compact|Indicates whether display labels from the next field in the same column on the Pivot Table view|
## Methods
| Name | Description |
| :- | :- |
|hide_item(index, is_hidden)|Sets whether the specific PivotItem in a data field is hidden.|
|hide_item(item_value, is_hidden)|Sets whether the specific PivotItem in a data field is hidden.|
|get_pivot_filter_by_type(type)|Gets the pivot filter of the pivot field by type|
|get_pivot_filters()|Gets the pivot filters of the pivot field|
|init_pivot_items()|Init the pivot items of the pivot field|
|get_calculated_field_formula()|Get the formula string of the specified calculated field .|
|set_subtotals(subtotal_type, shown)|Sets whether the specified field shows that subtotals.|
|get_subtotals(subtotal_type)|Gets whether the specified field shows that subtotals.|
|is_hidden_item(index)|Indicates whether the specific PivotItem is hidden.|
|is_hidden_item_detail(index)|Indicates whether the specific PivotItem is hidden detail.|
|hide_item_detail(index, is_hidden_detail)|Sets whether the specific PivotItem in a pivot field is hidden detail.|
|hide_detail(is_hidden_detail)|Sets whether the PivotItems in a pivot field is hidden detail.That is collapse/expand this field.|
|add_calculated_item(name, formula)|Add a calculated item to the pivot field.|

### See Also

* namespace [aspose.cells.pivot](/python-net/aspose.cells.pivot/)
* assembly [Aspose.Cells](/python-net/)

