##import_custom_objects method
## import_custom_objects(self, list, first_row, first_column, options) {#list-int-int-aspose.cells.ImportTableOptions}
Imports custom objects.
### Returns
Total number of rows imported.
```python
def import_custom_objects(self, list, first_row, first_column, options):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| list | list | The custom object |
| first_row | int | The row number of the first cell to import in. |
| first_column | int | The column number of the first cell to import in. |
| options | aspose.cells.ImportTableOptions | The import options. |
### Remarks
The custom objects should be the same type.
## import_custom_objects(self, list, property_names, is_property_name_shown, first_row, first_column, row_number, insert_rows, date_format_string, convert_string_to_number) {#list-list-bool-int-int-int-bool-System.String-bool}
Imports custom objects.
### Returns
Total number of rows imported.
```python
def import_custom_objects(self, list, property_names, is_property_name_shown, first_row, first_column, row_number, insert_rows, date_format_string, convert_string_to_number):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| list | list | The custom object |
| property_names | list | The property names.If it is null,we will import all properties of the object. |
| is_property_name_shown | bool | Indicates whether the property name will be imported to the first row. |
| first_row | int | The row number of the first cell to import in. |
| first_column | int | The column number of the first cell to import in. |
| row_number | int | Number of rows to be imported. |
| insert_rows | bool | Indicates whether extra rows are added to fit data. |
| date_format_string | System.String | Date format string for cells. |
| convert_string_to_number | bool | Indicates if this method will try to convert string to number. |
### Remarks
The custom objects should be the same type.
### See Also
* module [`aspose.cells`](../../)
* class [`Cells`](/cells/python-net/aspose.cells/cells)
