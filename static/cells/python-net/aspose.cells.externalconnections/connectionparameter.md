##ConnectionParameter class
## ConnectionParameter class
Specifies properties about any parameters used with external data connections
Parameters are valid for ODBC and web queries.
The ConnectionParameter type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [sql_type](/cells/python-net/aspose.cells.externalconnections/connectionparameter/sql_type) | SQL data type of the parameter. Only valid for ODBC sources. |
| [refresh_on_change](/cells/python-net/aspose.cells.externalconnections/connectionparameter/refresh_on_change) | Flag indicating whether the query should automatically refresh when the contents of a
| [prompt](/cells/python-net/aspose.cells.externalconnections/connectionparameter/prompt) | Prompt string for the parameter. Presented to the spreadsheet user along with input UI
| [type](/cells/python-net/aspose.cells.externalconnections/connectionparameter/type) | Type of parameter used.
| [name](/cells/python-net/aspose.cells.externalconnections/connectionparameter/name) | The name of the parameter. |
| [cell_reference](/cells/python-net/aspose.cells.externalconnections/connectionparameter/cell_reference) | Cell reference indicating which cell's value to use for the query parameter. Used only when parameterType is cell. |
| [value](/cells/python-net/aspose.cells.externalconnections/connectionparameter/value) | Non-integer numeric value,Integer value,String value or Boolean value
### See Also
* module [`aspose.cells.externalconnections`](..)
