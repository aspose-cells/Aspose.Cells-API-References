##GlobalizationSettings class
## GlobalizationSettings class
Represents the globalization settings.
The GlobalizationSettings type exposes the following members:
### Constructors
| Constructor | Description |
| :- | :- |
| [`__init__(self)`](/cells/python-net/aspose.cells/globalizationsettings/__init__/#) | Constructs a new instance of GlobalizationSettings |
### Properties
| Property | Description |
| :- | :- |
| [chart_settings](/cells/python-net/aspose.cells/globalizationsettings/chart_settings) | Gets or sets the globalization settings for Chart. |
| [pivot_settings](/cells/python-net/aspose.cells/globalizationsettings/pivot_settings) | Gets or sets the globalization settings for pivot table. |
| [list_separator](/cells/python-net/aspose.cells/globalizationsettings/list_separator) | Gets the separator for list, parameters of function, ...etc. |
| [row_separator_of_formula_array](/cells/python-net/aspose.cells/globalizationsettings/row_separator_of_formula_array) | Gets the separator for rows in array data in formula. |
| [column_separator_of_formula_array](/cells/python-net/aspose.cells/globalizationsettings/column_separator_of_formula_array) | Gets the separator for the items in array's row data in formula. |
### Methods
| Method | Description |
| :- | :- |
| [`get_pivot_total_name(self)`](/cells/python-net/aspose.cells/globalizationsettings/get_pivot_total_name/#) | Gets the name of "Total" label in the PivotTable.
| [`get_pivot_grand_total_name(self)`](/cells/python-net/aspose.cells/globalizationsettings/get_pivot_grand_total_name/#) | Gets the name of "Grand Total" label in the PivotTable. |
| [`get_multiple_items_name(self)`](/cells/python-net/aspose.cells/globalizationsettings/get_multiple_items_name/#) | Gets the name of "(Multiple Items)" label in the PivotTable. |
| [`get_all_name(self)`](/cells/python-net/aspose.cells/globalizationsettings/get_all_name/#) | Gets the name of "(All)" label in the PivotTable. |
| [`get_protection_name_of_pivot_table(self)`](/cells/python-net/aspose.cells/globalizationsettings/get_protection_name_of_pivot_table/#) | Gets the protection name in the PivotTable. |
| [`get_column_labels_of_pivot_table(self)`](/cells/python-net/aspose.cells/globalizationsettings/get_column_labels_of_pivot_table/#) | Gets the name of "Column Labels" label in the PivotTable. |
| [`get_row_labels_name_of_pivot_table(self)`](/cells/python-net/aspose.cells/globalizationsettings/get_row_labels_name_of_pivot_table/#) | Gets the name of "Row Labels" label in the PivotTable. |
| [`get_empty_data_name(self)`](/cells/python-net/aspose.cells/globalizationsettings/get_empty_data_name/#) | Gets the name of "(blank)" label in the PivotTable. |
| [`get_data_field_header_name_of_pivot_table(self)`](/cells/python-net/aspose.cells/globalizationsettings/get_data_field_header_name_of_pivot_table/#) | Gets the the name of the value area field header in the PivotTable. |
| [`get_sub_total_name(self, sub_total_type)`](/cells/python-net/aspose.cells/globalizationsettings/get_sub_total_name/#aspose.cells.pivot.pivotfieldsubtotaltype) | Gets the name of [`PivotFieldSubtotalType`](/cells/python-net/aspose.cells.pivot/pivotfieldsubtotaltype) type in the PivotTable. |
| [`get_total_name(self, function_type)`](/cells/python-net/aspose.cells/globalizationsettings/get_total_name/#aspose.cells.consolidationfunction) | Gets the total name of the function. |
| [`get_grand_total_name(self, function_type)`](/cells/python-net/aspose.cells/globalizationsettings/get_grand_total_name/#aspose.cells.consolidationfunction) | Gets the grand total name of the function. |
| [`get_default_sheet_name(self)`](/cells/python-net/aspose.cells/globalizationsettings/get_default_sheet_name/#) | Gets the default sheet name for adding worksheet automatically.
| [`get_table_row_type_of_headers(self)`](/cells/python-net/aspose.cells/globalizationsettings/get_table_row_type_of_headers/#) | Gets the type name of table rows that consists of the table header.
| [`get_table_row_type_of_data(self)`](/cells/python-net/aspose.cells/globalizationsettings/get_table_row_type_of_data/#) | Gets the type name of table rows that consists of data region of referenced table.
| [`get_table_row_type_of_all(self)`](/cells/python-net/aspose.cells/globalizationsettings/get_table_row_type_of_all/#) | Gets the type name of table rows that consists of all rows in referenced table.
| [`get_table_row_type_of_totals(self)`](/cells/python-net/aspose.cells/globalizationsettings/get_table_row_type_of_totals/#) | Gets the type name of table rows that consists of the total row of referenced table.
| [`get_table_row_type_of_current(self)`](/cells/python-net/aspose.cells/globalizationsettings/get_table_row_type_of_current/#) | Gets the type name of table rows that consists of the current row in referenced table.
| [`get_error_value_string(self, err)`](/cells/python-net/aspose.cells/globalizationsettings/get_error_value_string/#system.string) | Gets the display string value for cell's error value |
| [`get_boolean_value_string(self, bv)`](/cells/python-net/aspose.cells/globalizationsettings/get_boolean_value_string/#bool) | Gets the display string value for cell's boolean value |
| [`get_local_function_name(self, standard_name)`](/cells/python-net/aspose.cells/globalizationsettings/get_local_function_name/#system.string) | Gets the locale dependent function name according to given standard function name. |
| [`get_standard_function_name(self, local_name)`](/cells/python-net/aspose.cells/globalizationsettings/get_standard_function_name/#system.string) | Gets the standard function name according to given locale dependent function name. |
| [`get_local_built_in_name(self, standard_name)`](/cells/python-net/aspose.cells/globalizationsettings/get_local_built_in_name/#system.string) | Gets the locale dependent text for built-in Name according to given standard text. |
| [`get_standard_built_in_name(self, local_name)`](/cells/python-net/aspose.cells/globalizationsettings/get_standard_built_in_name/#system.string) | Gets the standard text of built-in Name according to given locale dependent text. |
| [`get_standard_header_footer_font_style_name(self, localfont_style_name)`](/cells/python-net/aspose.cells/globalizationsettings/get_standard_header_footer_font_style_name/#system.string) | Gets standard English font style name(Regular, Bold, Italic) for Header/Footer according to given locale font style name. |
| [`get_comment_title_name(self, type)`](/cells/python-net/aspose.cells/globalizationsettings/get_comment_title_name/#aspose.cells.rendering.commenttitletype) | Gets the locale dependent comment title name according to comment title type. |
| [`compare(self, v1, v2, ignore_case)`](/cells/python-net/aspose.cells/globalizationsettings/compare/#system.string-system.string-bool) | Compares two string values according to certain collation rules. |
### See Also
* module [`aspose.cells`](..)
* class [`PivotFieldSubtotalType`](/cells/python-net/aspose.cells.pivot/pivotfieldsubtotaltype)
