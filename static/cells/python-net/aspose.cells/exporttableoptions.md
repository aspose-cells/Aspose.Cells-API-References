##ExportTableOptions class
## ExportTableOptions class
Represents all export table options.
The ExportTableOptions type exposes the following members:
### Constructors
| Constructor | Description |
| :- | :- |
| [`__init__(self)`](/cells/python-net/aspose.cells/exporttableoptions/__init__/#) | Constructs a new instance of ExportTableOptions |
### Properties
| Property | Description |
| :- | :- |
| [export_column_name](/cells/python-net/aspose.cells/exporttableoptions/export_column_name) | Indicates whether the data in the first row are exported to the column name of the DataTable.
| [skip_error_value](/cells/python-net/aspose.cells/exporttableoptions/skip_error_value) | Indicates whether skip invalid value for the column.
| [plot_visible_cells](/cells/python-net/aspose.cells/exporttableoptions/plot_visible_cells) | Only exports visible cells. |
| [plot_visible_rows](/cells/python-net/aspose.cells/exporttableoptions/plot_visible_rows) | Only exports visible rows. |
| [plot_visible_columns](/cells/python-net/aspose.cells/exporttableoptions/plot_visible_columns) | Only exports visible columns. |
| [export_as_string](/cells/python-net/aspose.cells/exporttableoptions/export_as_string) | Exports the string value of the cells to the DataTable. |
| [export_as_html_string](/cells/python-net/aspose.cells/exporttableoptions/export_as_html_string) | Exports the html string value of the cells to the DataTable. |
| [format_strategy](/cells/python-net/aspose.cells/exporttableoptions/format_strategy) | Gets and sets the format strategy when exporting the value as string value. |
| [check_mixed_value_type](/cells/python-net/aspose.cells/exporttableoptions/check_mixed_value_type) | False, Aspose.Cells will set the DataColumn's type by the value type of the first row for performance.
| [allow_db_null](/cells/python-net/aspose.cells/exporttableoptions/allow_db_null) | This value indicates whether DBNulls are allowed in this table. |
| [is_vertical](/cells/python-net/aspose.cells/exporttableoptions/is_vertical) | True if a row in Workbook file represents a row in DataTable. False if a column in Workbook file represents a row in DataTable. |
| [indexes](/cells/python-net/aspose.cells/exporttableoptions/indexes) | The indexes of columns/rows which should be exported out. |
| [rename_strategy](/cells/python-net/aspose.cells/exporttableoptions/rename_strategy) | Strategy for duplicate names of columns. |
### Methods
| Method | Description |
| :- | :- |
| [`preprocess_exported_value(self, cell_row, cell_column, value)`](/cells/python-net/aspose.cells/exporttableoptions/preprocess_exported_value/#int-int-aspose.cells.cellvalue) | Preprocess the value of current cell to be exported. |
### Remarks
If there are some special requirements about the exporting, such as ignoring error values, user may extend this class
to overwrite corresponding apis to achive the goal.
### See Also
* module [`aspose.cells`](..)
