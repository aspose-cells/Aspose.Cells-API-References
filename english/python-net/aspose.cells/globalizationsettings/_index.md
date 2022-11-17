---
title: GlobalizationSettings
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 730
url: /python-net/aspose.cells/globalizationsettings/
---

## GlobalizationSettings class

Represents the globalization settings.

The GlobalizationSettings type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|GlobalizationSettings()|Initializes a new instance of the GlobalizationSettings class|
## Properties
| Name | Description |
| :- | :- |
|chart_settings|Gets or sets the Chart of this[ChartGlobalizationSettings](/cells/python-net/aspose.cells.charts/chartglobalizationsettings/)|
|list_separator|Gets the separator for list, parameters of function, ...etc.|
|row_separator_of_formula_array|Gets the separator for rows in array data in formula.|
|column_separator_of_formula_array|Gets the separator for the items in array's row data in formula.|
## Methods
| Name | Description |
| :- | :- |
|compare(v1, v2, ignore_case)|Compares two string values according to certain collation rules.|
|get_pivot_total_name()|Gets the name of "Total" label in the PivotTable.<br/>            You need to override this method when the PivotTable contains two or more PivotFields in the data area.|
|get_pivot_grand_total_name()|Gets the name of "Grand Total" label in the PivotTable.|
|get_multiple_items_name()|Gets the name of "(Multiple Items)" label in the PivotTable.|
|get_all_name()|Gets the name of "(All)" label in the PivotTable.|
|get_column_lables_name()|Gets the name of "Column Labels" label in the PivotTable.|
|get_row_lables_name()|Gets the name of "Row Labels" label in the PivotTable.|
|get_protection_name_of_pivot_table()|Gets the protection name in the PivotTable.|
|get_column_labels_of_pivot_table()|Gets the name of "Column Labels" label in the PivotTable.|
|get_row_labels_name_of_pivot_table()|Gets the name of "Row Labels" label in the PivotTable.|
|get_empty_data_name()|Gets the name of "(blank)" label in the PivotTable.|
|get_sub_total_name(sub_total_type)|Gets the name of [PivotFieldSubtotalType](/cells/python-net/aspose.cells.pivot/pivotfieldsubtotaltype/) type in the PivotTable.|
|get_total_name(function_type)|Gets the total name of the function.|
|get_grand_total_name(function_type)|Gets the grand total name of the function.|
|get_other_name()|Gets the name of "Other" labels for Pie charts.|
|get_table_row_type_of_headers()|Gets the type name of table rows that consists of the table header.<br/>            Default is "Headers", so in formula "#Headers" represents the table header.|
|get_table_row_type_of_data()|Gets the type name of table rows that consists of data region of referenced table.<br/>            Default is "Data", so in formula "#Data" represents the data region of the table.|
|get_table_row_type_of_all()|Gets the type name of table rows that consists of all rows in referenced table.<br/>            Default is "All", so in formula "#All" represents all rows in referenced table.|
|get_table_row_type_of_totals()|Gets the type name of table rows that consists of the total row of referenced table.<br/>            Default is "Totals", so in formula "#Totals" represents the total row of referenced table.|
|get_table_row_type_of_current()|Gets the type name of table rows that consists of the current row in referenced table.<br/>            Default is "This Row", so in formula "#This Row" represents the current row in referenced table.|
|get_error_value_string(err)|Gets the display string value for cell's error value|
|get_boolean_value_string(bv)|Gets the display string value for cell's boolean value|
|get_local_function_name(standard_name)|Gets the locale dependent function name according to given standard function name.|
|get_standard_function_name(local_name)|Gets the standard function name according to given locale dependent function name.|
|get_local_built_in_name(standard_name)|Gets the locale dependent text for built-in Name according to given standard text.|
|get_standard_built_in_name(local_name)|Gets the standard text of built-in Name according to given locale dependent text.|
|get_standard_header_footer_font_style_name(localfont_style_name)|Gets standard English font style name(Regular, Bold, Italic) for Header/Footer according to given locale font style name.|
|get_comment_title_name(type)|Gets the locale dependent comment title name according to comment title type.|

### See Also

* namespace [aspose.cells](/cells/python-net/aspose.cells/)
* assembly [Aspose.Cells](/cells/python-net/)

