---
title: PivotTable
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 100
url: /cells/python-net/aspose.cells.pivot/pivottable/
---

## PivotTable class

Summary description for PivotTable.

The PivotTable type exposes the following members:
## Properties
| Name | Description |
| :- | :- |
|is_excel_2003_compatible|Specifies whether the PivotTable is compatible for Excel2003 when refreshing PivotTable,<br/>            if true, a string must be less than or equal to 255 characters, so if the string is greater than 255 characters,<br/>            it will be truncated. if false, a string will not have the aforementioned restriction.<br/>            The default value is true.|
|refreshed_by_who|Gets the name of the user who last refreshed the PivotTable|
|refresh_date|Gets the date when the PivotTable was last refreshed.|
|pivot_table_style_name|Gets and sets the pivottable style name.|
|pivot_table_style_type|Gets and sets the built-in pivot table style.|
|column_fields|Returns a PivotFields object that are currently shown as column fields.|
|row_fields|Returns a PivotFields object that are currently shown as row fields.|
|page_fields|Returns a PivotFields object that are currently shown as page fields.|
|data_fields|Gets a PivotField object that represents all the data fields in a PivotTable.<br/>            Read-only.It would be init only when there are two or more data fields in the DataPiovtFiels.<br/>            It only use to add DataPivotField to the PivotTable row/column area . Default is in row area.|
|data_field|Gets a PivotField object that represents all the data fields in a PivotTable.<br/>            Read-only.It would be init only when there are two or more data fields in the DataPiovtFiels.<br/>            It only use to add DataPivotField to the PivotTable row/column area . Default is in row area.|
|base_fields|Returns a PivotFields object that includes all fields in the PivotTable report|
|pivot_filters|Returns a PivotFilterCollection object.|
|column_range|Returns a CellArea object that represents the range<br/>            that contains the column area in the PivotTable report. Read-only.|
|row_range|Returns a CellArea object that represents the range<br/>            that contains the row area in the PivotTable report. Read-only.|
|data_body_range|Returns a CellArea object that represents the range that contains the data area<br/>            in the list between the header row and the insert row. Read-only.|
|table_range1|Returns a CellArea object that represents the range containing the entire PivotTable report,<br/>            but doesn't include page fields. Read-only.|
|table_range2|Returns a CellArea object that represents the range containing the entire PivotTable report,<br/>            includes page fields. Read-only.|
|column_grand|Indicates whether the PivotTable report shows grand totals for columns.|
|is_grid_drop_zones|Indicates whether the PivotTable report displays classic pivottable layout.<br/>            (enables dragging fields in the grid)|
|row_grand|Indicates whether the PivotTable report shows grand totals for rows.|
|display_null_string|Indicates whether the PivotTable report displays a custom string<br/>            in cells that contain null values.|
|null_string|Gets the string displayed in cells that contain null values<br/>            when the DisplayNullString property is true.The default value is an empty string.|
|display_error_string|Indicates whether the PivotTable report displays a custom string in cells that contain errors.|
|error_string|Gets the string displayed in cells that contain errors<br/>            when the DisplayErrorString property is true.The default value is an empty string.|
|is_auto_format|Indicates whether the PivotTable report is automatically formatted.<br/>            Checkbox "autoformat table " which is in pivottable option for Excel 2003<br/>            Checkbox "autofit column width on update" which is in pivot table Options :Layout Format for Excel 2007|
|auto_format_type|Gets the PivotTable auto format type.|
|has_blank_rows|Indicates whether to add blank rows.<br/>            This property only applies for the PivotTable auto format types which needs to add blank rows.|
|merge_labels|Indicates whether the specified PivotTable report's outer-row item, column item, subtotal,<br/>            and grand total labels use merged cells.|
|preserve_formatting|Indicates whether formatting is preserved when the PivotTable is refreshed or recalculated.|
|show_drill|Gets whether expand/collapse buttons is shown.|
|enable_drilldown|Gets whether drilldown is enabled.|
|enable_field_dialog|Indicates whether the PivotTable Field dialog box is available<br/>            when the user double-clicks the PivotTable field.|
|enable_field_list|Gets whether enable the field list for the PivotTable.|
|enable_wizard|Indicates whether the PivotTable Wizard is available.|
|subtotal_hidden_page_items|Indicates whether hidden page field items in the PivotTable report<br/>             are included in row and column subtotals, block totals, and grand totals.<br/>             The default value is False.|
|grand_total_name|Returns the text string label that is displayed in the grand total column or row heading.<br/>            The default value is the string "Grand Total".|
|manual_update|Indicates whether the PivotTable report is recalculated only at the user's request.|
|is_multiple_field_filters|Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them.|
|missing_items_limit|Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them.|
|enable_data_value_editing|Specifies a boolean value that indicates whether the user is allowed to edit the cells in the data area of the pivottable.<br/>            Enable cell editing in the values area|
|show_data_tips|Specifies a boolean value that indicates whether tooltips should be displayed for PivotTable data cells.|
|show_member_property_tips|Specifies a boolean value that indicates whether member property information should be omitted from PivotTable tooltips.|
|show_values_row|Specifies a boolean value that indicates whether show values row.<br/>             show the values row|
|show_empty_col|Specifies a boolean value that indicates whether to include empty columns in the table|
|show_empty_row|Specifies a boolean value that indicates whether to include empty rows in the table.|
|field_list_sort_ascending|Specifies a boolean value that indicates whether fields in the PivotTable are sorted in non-default order in the field list.|
|print_drill|Specifies a boolean value that indicates whether drill indicators should be printed.<br/>            print expand/collapse buttons when displayed on pivottable.|
|alt_text_title|Gets the title of the altertext|
|alt_text_description|Gets the description of the alt text|
|name|Gets the name of the PivotTable|
|column_header_caption|Gets the Column Header Caption of the PivotTable.|
|indent|Specifies the indentation increment for compact axis and can be used to set the Report Layout to Compact Form.|
|row_header_caption|Gets the Row Header Caption of the PivotTable.|
|show_row_header_caption|Indicates whether row header caption is shown in the PivotTable report<br/>             Indicates whether Display field captions and filter drop downs|
|custom_list_sort|Indicates whether consider built-in custom list when sort data|
|pivot_format_conditions|Gets the Format Conditions of the pivot table.|
|page_field_order|Gets the order in which page fields are added to the PivotTable report's layout.|
|page_field_wrap_count|Gets the number of page fields in each column or row in the PivotTable report.|
|tag|Gets a string saved with the PivotTable report.|
|save_data|Indicates whether data for the PivotTable report is saved with the workbook.|
|refresh_data_on_opening_file|Indicates whether Refresh Data when Opening File.|
|refresh_data_flag|Indicates whether Refresh Data or not.|
|external_connection_data_source|Gets the external connection data source.|
|data_source|Gets and sets the data source of the pivot table.|
|item_print_titles|A bit that specifies whether pivot item captions on the row axis<br/>            are repeated on each printed page for pivot fields in tabular form.|
|print_titles|Indicates whether the print titles for the worksheet are set based<br/>            on the PivotTable report. The default value is false.|
|display_immediate_items|Indicates whether items in the row and column areas are visible<br/>            when the data area of the PivotTable is empty. The default value is true.|
|is_selected|Indicates whether the PivotTable is selected.|
|show_pivot_style_row_header|Indicates whether the row header in the pivot table should have the style applied.|
|show_pivot_style_column_header|Indicates whether the column header in the pivot table should have the style applied.|
|show_pivot_style_row_stripes|Indicates whether row stripe formatting is applied.|
|show_pivot_style_column_stripes|Indicates whether column stripe formatting is applied.|
|show_pivot_style_last_column|Indicates whether column stripe formatting is applied.|
## Methods
| Name | Description |
| :- | :- |
|remove_field(field_type, field_name)|Removes a field from specific field area|
|remove_field(field_type, base_field_index)|Removes a field from specific field area|
|remove_field(field_type, pivot_field)|Removes a field from specific field area|
|add_field_to_area(field_type, field_name)|Adds the field to the specific area.|
|add_field_to_area(field_type, base_field_index)|Adds the field to the specific area.|
|add_field_to_area(field_type, pivot_field)|Adds the field to the specific area.|
|add_calculated_field(name, formula, drag_to_data_area)|Adds a calculated field to pivot field.|
|add_calculated_field(name, formula)|Adds a calculated field to pivot field.|
|move(row, column)|Moves the PivotTable to a different location in the worksheet.|
|move(dest_cell_name)|Moves the PivotTable to a different location in the worksheet.|
|set_auto_group_field(base_field_index)|Sets auto field group by the PivotTable.|
|set_auto_group_field(pivot_field)|Sets auto field group by the PivotTable.|
|set_manual_group_field(base_field_index, start_val, end_val, group_by_list, interval_num)|Sets manual field group by the PivotTable.|
|set_manual_group_field(pivot_field, start_val, end_val, group_by_list, interval_num)|Sets manual field group by the PivotTable.|
|set_manual_group_field(base_field_index, start_val, end_val, group_by_list, interval_num)|Sets manual field group by the PivotTable.|
|set_manual_group_field(pivot_field, start_val, end_val, group_by_list, interval_num)|Sets manual field group by the PivotTable.|
|set_ungroup(base_field_index)|Sets ungroup by the PivotTable|
|set_ungroup(pivot_field)|Sets ungroup by the PivotTable|
|copy_style(pivot_table)|Copies named style from another pivot table.|
|show_report_filter_page(page_field)|Show all the report filter pages according to PivotField, the PivotField must be located in the PageFields.|
|show_report_filter_page_by_name(field_name)|Show all the report filter pages according to PivotField's name, the PivotField must be located in the PageFields.|
|show_report_filter_page_by_index(pos_index)|Show all the report filter pages according to the position index in the PageFields|
|fields(field_type)|Gets the specific fields by the field type.|
|change_data_source(source)|Set pivottable's source data.<br/>            Sheet1!$A$1:$C$3|
|get_source()|Get pivottable's source data.|
|refresh_data()|Refreshes pivottable's data and setting from it's data source.|
|calculate_data()|Calculates pivottable's data to cells.|
|clear_data()|Clear PivotTable's data and formatting|
|calculate_range()|Calculates pivottable's range.|
|format_all(style)|Format all the cell in the pivottable area|
|format_row(row, style)|Format the row data in the pivottable area|
|format(row, column, style)|Format the row data in the pivottable area|
|get_horizontal_breaks()|get pivot table row index list of horizontal pagebreaks|
|show_in_compact_form()|Layouts the PivotTable in compact form.|
|show_in_outline_form()|Layouts the PivotTable in outline form.|
|show_in_tabular_form()|Layouts the PivotTable in tabular form.|
|get_cell_by_display_name(display_name)|Gets the Cell object by the DisplayName of PivotField|
|get_children()|Gets the Children Pivot Tables which use this PivotTable data as data source.|

### See Also

* namespace [aspose.cells.pivot](/cells/python-net/aspose.cells.pivot/)
* assembly [Aspose.Cells](/cells/python-net/)

