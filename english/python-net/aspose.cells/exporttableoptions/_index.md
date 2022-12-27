---
title: ExportTableOptions class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 550
url: /python-net/aspose.cells/exporttableoptions/
is_root: false
---

## ExportTableOptions class

Represents all export table options.



The ExportTableOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [ExportTableOptions()](/cells/python-net/aspose.cells/exporttableoptions/__init__/#) |  |


### Properties
| Property | Description |
| :- | :- |
| [export_column_name](/cells/python-net/aspose.cells/exporttableoptions/export_column_name) | Indicates whether the data in the first row are exported to the column name of the DataTable.<br/>The default value is false. |
| [skip_error_value](/cells/python-net/aspose.cells/exporttableoptions/skip_error_value) | Indicates whether skip invalid value for the column.<br/>For example,if the column type is decimal ,the value is greater than decimal.MaxValue <br/>and this property is true,we will not throw exception again.<br/>The default value is false. |
| [plot_visible_cells](/cells/python-net/aspose.cells/exporttableoptions/plot_visible_cells) | Only exports visible cells. |
| [plot_visible_rows](/cells/python-net/aspose.cells/exporttableoptions/plot_visible_rows) | Only exports visible rows. |
| [plot_visible_columns](/cells/python-net/aspose.cells/exporttableoptions/plot_visible_columns) | Only exports visible columns. |
| [export_as_string](/cells/python-net/aspose.cells/exporttableoptions/export_as_string) | Exports the string value of the cells to the DataTable. |
| [export_as_html_string](/cells/python-net/aspose.cells/exporttableoptions/export_as_html_string) | Exports the html string value of the cells to the DataTable. |
| [format_strategy](/cells/python-net/aspose.cells/exporttableoptions/format_strategy) | Gets and sets the format strategy when exporting the value as string value. |
| [check_mixed_value_type](/cells/python-net/aspose.cells/exporttableoptions/check_mixed_value_type) | False, Aspose.Cells will set the DataColumn's type by the value type of the first row for performance.<br/>True, Aspose.Cells will check whether the value type in the column are mixed before set the DataColumn's type <br/>And the value type are mixed, the DataColumn's type will be string. |
| [is_vertical](/cells/python-net/aspose.cells/exporttableoptions/is_vertical) | True if a row in Workbook file represents a row in DataTable. False if a column in Workbook file represents a row in DataTable. |
| [indexes](/cells/python-net/aspose.cells/exporttableoptions/indexes) | The indexes of columns/rows which should be exported out. |
| [rename_strategy](/cells/python-net/aspose.cells/exporttableoptions/rename_strategy) | Strategy for duplicate names of columns. |


### See Also

* module [aspose.cells](../)
