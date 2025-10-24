##SettableGlobalizationSettings class
## SettableGlobalizationSettings class
Implementation of GlobalizationSettings that supports user to set/change pre-defined texts.
**Inheritance:** [`SettableGlobalizationSettings`](/cells/python-net/aspose.cells/settableglobalizationsettings) →
[`GlobalizationSettings`](/cells/python-net/aspose.cells/globalizationsettings)
The SettableGlobalizationSettings type exposes the following members:
### Constructors
| Constructor | Description |
| :- | :- |
| [`__init__(self)`](/cells/python-net/aspose.cells/settableglobalizationsettings/__init__/#) | Constructs a new instance of SettableGlobalizationSettings |
### Properties
| Property | Description |
| :- | :- |
| [chart_settings](/cells/python-net/aspose.cells/settableglobalizationsettings/chart_settings) | Gets or sets the globalization settings for Chart. |
| [pivot_settings](/cells/python-net/aspose.cells/settableglobalizationsettings/pivot_settings) | Gets or sets the globalization settings for pivot table. |
| [list_separator](/cells/python-net/aspose.cells/settableglobalizationsettings/list_separator) | Gets the separator for list, parameters of function, ...etc. |
| [row_separator_of_formula_array](/cells/python-net/aspose.cells/settableglobalizationsettings/row_separator_of_formula_array) | Gets the separator for rows in array data in formula. |
| [column_separator_of_formula_array](/cells/python-net/aspose.cells/settableglobalizationsettings/column_separator_of_formula_array) | Gets the separator for the items in array's row data in formula. |
### Methods
| Method | Description |
| :- | :- |
| [`get_pivot_total_name(self)`](/cells/python-net/aspose.cells/settableglobalizationsettings/get_pivot_total_name/#) | Gets the name of "Total" label in the PivotTable.
| [`get_pivot_grand_total_name(self)`](/cells/python-net/aspose.cells/settableglobalizationsettings/get_pivot_grand_total_name/#) | Gets the name of "Grand Total" label in the PivotTable. |
| [`get_multiple_items_name(self)`](/cells/python-net/aspose.cells/settableglobalizationsettings/get_multiple_items_name/#) | Gets the name of "(Multiple Items)" label in the PivotTable. |
| [`get_all_name(self)`](/cells/python-net/aspose.cells/settableglobalizationsettings/get_all_name/#) | Gets the name of "(All)" label in the PivotTable. |
| [`get_protection_name_of_pivot_table(self)`](/cells/python-net/aspose.cells/settableglobalizationsettings/get_protection_name_of_pivot_table/#) | Gets the protection name in the PivotTable. |
| [`get_column_labels_of_pivot_table(self)`](/cells/python-net/aspose.cells/settableglobalizationsettings/get_column_labels_of_pivot_table/#) | Gets the name of "Column Labels" label in the PivotTable. |
| [`get_row_labels_name_of_pivot_table(self)`](/cells/python-net/aspose.cells/settableglobalizationsettings/get_row_labels_name_of_pivot_table/#) | Gets the name of "Row Labels" label in the PivotTable. |
| [`get_empty_data_name(self)`](/cells/python-net/aspose.cells/settableglobalizationsettings/get_empty_data_name/#) | Gets the name of "(blank)" label in the PivotTable. |
| [`get_data_field_header_name_of_pivot_table(self)`](/cells/python-net/aspose.cells/settableglobalizationsettings/get_data_field_header_name_of_pivot_table/#) | Gets the the name of the value area field header in the PivotTable. |
| [`get_sub_total_name(self, sub_total_type)`](/cells/python-net/aspose.cells/settableglobalizationsettings/get_sub_total_name/#aspose.cells.pivot.pivotfieldsubtotaltype) | Gets the name of [`PivotFieldSubtotalType`](/cells/python-net/aspose.cells.pivot/pivotfieldsubtotaltype) type in the PivotTable. |
| [`get_total_name(self, function_type)`](/cells/python-net/aspose.cells/settableglobalizationsettings/get_total_name/#aspose.cells.consolidationfunction) | Gets the total name of specific function. |
| [`get_grand_total_name(self, function_type)`](/cells/python-net/aspose.cells/settableglobalizationsettings/get_grand_total_name/#aspose.cells.consolidationfunction) | Gets the grand total name of the function. |
| [`get_default_sheet_name(self)`](/cells/python-net/aspose.cells/settableglobalizationsettings/get_default_sheet_name/#) | Gets the default sheet name for adding worksheet automatically.
| [`get_table_row_type_of_headers(self)`](/cells/python-net/aspose.cells/settableglobalizationsettings/get_table_row_type_of_headers/#) | Gets the type name of table rows that consists of the table header.
| [`get_table_row_type_of_data(self)`](/cells/python-net/aspose.cells/settableglobalizationsettings/get_table_row_type_of_data/#) | Gets the type name of table rows that consists of data region of referenced table.
| [`get_table_row_type_of_all(self)`](/cells/python-net/aspose.cells/settableglobalizationsettings/get_table_row_type_of_all/#) | Gets the type name of table rows that consists of all rows in referenced table. |
| [`get_table_row_type_of_totals(self)`](/cells/python-net/aspose.cells/settableglobalizationsettings/get_table_row_type_of_totals/#) | Gets the type name of table rows that consists of the total row of referenced table. |
| [`get_table_row_type_of_current(self)`](/cells/python-net/aspose.cells/settableglobalizationsettings/get_table_row_type_of_current/#) | Gets the type name of table rows that consists of the current row in referenced table. |
| [`get_error_value_string(self, err)`](/cells/python-net/aspose.cells/settableglobalizationsettings/get_error_value_string/#system.string) | Gets the display string value for cell's error value |
| [`get_boolean_value_string(self, bv)`](/cells/python-net/aspose.cells/settableglobalizationsettings/get_boolean_value_string/#bool) | Gets the display string value for cell's boolean value |
| [`get_local_function_name(self, standard_name)`](/cells/python-net/aspose.cells/settableglobalizationsettings/get_local_function_name/#system.string) | Gets the locale dependent function name according to given standard function name. |
| [`get_standard_function_name(self, local_name)`](/cells/python-net/aspose.cells/settableglobalizationsettings/get_standard_function_name/#system.string) | Gets the standard function name according to given locale dependent function name. |
| [`get_local_built_in_name(self, standard_name)`](/cells/python-net/aspose.cells/settableglobalizationsettings/get_local_built_in_name/#system.string) | Gets the locale dependent text for built-in Name according to given standard text. |
| [`get_standard_built_in_name(self, local_name)`](/cells/python-net/aspose.cells/settableglobalizationsettings/get_standard_built_in_name/#system.string) | Gets the standard text of built-in Name according to given locale dependent text. |
| [`get_standard_header_footer_font_style_name(self, localfont_style_name)`](/cells/python-net/aspose.cells/settableglobalizationsettings/get_standard_header_footer_font_style_name/#system.string) | Gets standard English font style name(Regular, Bold, Italic) for Header/Footer according to given locale font style name. |
| [`get_comment_title_name(self, type)`](/cells/python-net/aspose.cells/settableglobalizationsettings/get_comment_title_name/#aspose.cells.rendering.commenttitletype) | Gets the locale dependent comment title name according to comment title type. |
| [`compare(self, v1, v2, ignore_case)`](/cells/python-net/aspose.cells/settableglobalizationsettings/compare/#system.string-system.string-bool) | Compares two string values according to certain collation rules. |
| [`set_total_name(self, function_type, name)`](/cells/python-net/aspose.cells/settableglobalizationsettings/set_total_name/#aspose.cells.consolidationfunction-system.string) | Sets the total name of specific function. |
| [`set_grand_total_name(self, function_type, name)`](/cells/python-net/aspose.cells/settableglobalizationsettings/set_grand_total_name/#aspose.cells.consolidationfunction-system.string) | Sets the grand total name of specific function. |
| [`set_table_row_type_of_headers(self, name)`](/cells/python-net/aspose.cells/settableglobalizationsettings/set_table_row_type_of_headers/#system.string) | Sets the type name of table rows that consists of the table header. |
| [`set_table_row_type_of_data(self, name)`](/cells/python-net/aspose.cells/settableglobalizationsettings/set_table_row_type_of_data/#system.string) | Sets the type name of table rows that consists of data region of referenced table. |
| [`set_table_row_type_of_all(self, name)`](/cells/python-net/aspose.cells/settableglobalizationsettings/set_table_row_type_of_all/#system.string) | Sets the type name of table rows that consists of all rows in referenced table. |
| [`set_table_row_type_of_totals(self, name)`](/cells/python-net/aspose.cells/settableglobalizationsettings/set_table_row_type_of_totals/#system.string) | Sets the type name of table rows that consists of the total row of referenced table. |
| [`set_table_row_type_of_current(self, name)`](/cells/python-net/aspose.cells/settableglobalizationsettings/set_table_row_type_of_current/#system.string) | Sets the type name of table rows that consists of the current row in referenced table. |
| [`set_boolean_value_string(self, bv, name)`](/cells/python-net/aspose.cells/settableglobalizationsettings/set_boolean_value_string/#bool-system.string) | Sets the display string value for cell's boolean value |
| [`set_local_function_name(self, standard_name, local_name, bidirectional)`](/cells/python-net/aspose.cells/settableglobalizationsettings/set_local_function_name/#system.string-system.string-bool) | Sets the locale dependent function name corresponding to given standard function name. |
| [`set_standard_function_name(self, local_name, standard_name, bidirectional)`](/cells/python-net/aspose.cells/settableglobalizationsettings/set_standard_function_name/#system.string-system.string-bool) | Sets the locale dependent function name according to given standard function name. |
| [`set_local_built_in_name(self, standard_name, local_name, bidirectional)`](/cells/python-net/aspose.cells/settableglobalizationsettings/set_local_built_in_name/#system.string-system.string-bool) | Sets the locale dependent text for the built-in name with given standard name text. |
| [`set_standard_built_in_name(self, local_name, standard_name, bidirectional)`](/cells/python-net/aspose.cells/settableglobalizationsettings/set_standard_built_in_name/#system.string-system.string-bool) | Sets the locale dependent function name according to given standard function name. |
| [`set_list_separator(self, c)`](/cells/python-net/aspose.cells/settableglobalizationsettings/set_list_separator/#system.char) | Sets the separator for list, parameters of function, ...etc. |
| [`set_row_separator_of_formula_array(self, c)`](/cells/python-net/aspose.cells/settableglobalizationsettings/set_row_separator_of_formula_array/#system.char) | Sets the separator for rows in array data in formula. |
| [`set_column_separator_of_formula_array(self, c)`](/cells/python-net/aspose.cells/settableglobalizationsettings/set_column_separator_of_formula_array/#system.char) | Sets the separator for the items in array's row data in formula. |
| [`set_standard_header_footer_font_style_name(self, localfont_style_name, standard_name)`](/cells/python-net/aspose.cells/settableglobalizationsettings/set_standard_header_footer_font_style_name/#system.string-system.string) | Sets the locale dependent function name according to given standard function name. |
| [`set_comment_title_name(self, type, name)`](/cells/python-net/aspose.cells/settableglobalizationsettings/set_comment_title_name/#aspose.cells.rendering.commenttitletype-system.string) | Gets the locale dependent comment title name according to comment title type. |
### See Also
* module [`aspose.cells`](..)
* class [`GlobalizationSettings`](/cells/python-net/aspose.cells/globalizationsettings)
* class [`PivotFieldSubtotalType`](/cells/python-net/aspose.cells.pivot/pivotfieldsubtotaltype)
* class [`SettableGlobalizationSettings`](/cells/python-net/aspose.cells/settableglobalizationsettings)
