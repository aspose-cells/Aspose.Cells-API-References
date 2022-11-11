---
title: ExportTableOptions
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 550
url: /cells/python-net/aspose.cells/exporttableoptions/
---

## ExportTableOptions class

Represents all export table options.

The ExportTableOptions type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|ExportTableOptions()|Initializes a new instance of the ExportTableOptions class|
## Properties
| Name | Description |
| :- | :- |
|export_column_name|Indicates whether the data in the first row are exported to the column name of the DataTable.<br/>            The default value is false.|
|skip_error_value|Indicates whether skip invalid value for the column.<br/>             For example,if the column type is decimal ,the value is greater than decimal.MaxValue <br/>             and this property is true,we will not throw exception again.<br/>             The default value is false.|
|plot_visible_cells|Only exports visible cells.|
|plot_visible_rows|Only exports visible rows.|
|plot_visible_columns|Only exports visible columns.|
|export_as_string|Exports the string value of the cells to the DataTable.|
|export_as_html_string|Exports the html string value of the cells to the DataTable.|
|format_strategy|Gets and sets the format strategy when exporting the value as string value.|
|check_mixed_value_type|False, Aspose.Cells will set the DataColumn's type by the value type of the first row for performance.<br/>            True, Aspose.Cells will check whether the value type in the column are mixed before set the DataColumn's type <br/>            And the value type are mixed, the DataColumn's type will be string.|
|is_vertical|True if a row in Workbook file represents a row in DataTable. False if a column in Workbook file represents a row in DataTable.|
|indexes|The indexes of columns/rows which should be exported out.|
|rename_strategy|Strategy for duplicate names of columns.|

### See Also

* namespace [aspose.cells](/cells/python-net/aspose.cells/)
* assembly [Aspose.Cells](/cells/python-net/)

