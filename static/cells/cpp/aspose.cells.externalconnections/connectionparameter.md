##Aspose::Cells::ExternalConnections::ConnectionParameter class
'Aspose::Cells::ExternalConnections::ConnectionParameter class. Specifies properties about any parameters used with external data connections Parameters are valid for ODBC and web queries in C++.'
## ConnectionParameter class
Specifies properties about any parameters used with external data connections Parameters are valid for ODBC and web queries.
```cpp
class ConnectionParameter
```
## Methods
| Method | Description |
| --- | --- |
| [ConnectionParameter(ConnectionParameter_Impl* impl)](./connectionparameter/) | Constructs from an implementation object. |
| [ConnectionParameter(const ConnectionParameter\& src)](./connectionparameter/) | Copy constructor. |
| [GetCellReference()](./getcellreference/) | [Cell](../../aspose.cells/cell/) reference indicating which cell's value to use for the query parameter. Used only when parameterType is cell. |
| [GetName()](./getname/) | The name of the parameter. |
| [GetPrompt()](./getprompt/) | Prompt string for the parameter. Presented to the spreadsheet user along with input UI to collect the parameter value before refreshing the external data. Used only when parameterType = prompt. |
| [GetRefreshOnChange()](./getrefreshonchange/) | Flag indicating whether the query should automatically refresh when the contents of a cell that provides the parameter value changes. If true, then external data is refreshed using the new parameter value every time there's a change. If false, then external data is only refreshed when requested by the user, or some other event triggers refresh (e.g., workbook opened). |
| [GetSqlType()](./getsqltype/) | SQL data type of the parameter. Only valid for ODBC sources. |
| [GetType()](./gettype/) | Type of parameter used. If the parameterType=value, then the value from boolean, double, integer, or string will be used. In this case, it is expected that only one of {boolean, double, integer, or string} will be specified. |
| [GetValue()](./getvalue/) | Non-integer numeric value,Integer value,String value or Boolean value to use as the query parameter. Used only when parameterType is value. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ConnectionParameter\& src)](./operator_asm/) | operator= |
| [SetCellReference(const U16String\& value)](./setcellreference/) | [Cell](../../aspose.cells/cell/) reference indicating which cell's value to use for the query parameter. Used only when parameterType is cell. |
| [SetCellReference(const char16_t* value)](./setcellreference/) | [Cell](../../aspose.cells/cell/) reference indicating which cell's value to use for the query parameter. Used only when parameterType is cell. |
| [SetName(const U16String\& value)](./setname/) | The name of the parameter. |
| [SetName(const char16_t* value)](./setname/) | The name of the parameter. |
| [SetPrompt(const U16String\& value)](./setprompt/) | Prompt string for the parameter. Presented to the spreadsheet user along with input UI to collect the parameter value before refreshing the external data. Used only when parameterType = prompt. |
| [SetPrompt(const char16_t* value)](./setprompt/) | Prompt string for the parameter. Presented to the spreadsheet user along with input UI to collect the parameter value before refreshing the external data. Used only when parameterType = prompt. |
| [SetRefreshOnChange(bool value)](./setrefreshonchange/) | Flag indicating whether the query should automatically refresh when the contents of a cell that provides the parameter value changes. If true, then external data is refreshed using the new parameter value every time there's a change. If false, then external data is only refreshed when requested by the user, or some other event triggers refresh (e.g., workbook opened). |
| [SetSqlType(SqlDataType value)](./setsqltype/) | SQL data type of the parameter. Only valid for ODBC sources. |
| [SetType(ConnectionParameterType value)](./settype/) | Type of parameter used. If the parameterType=value, then the value from boolean, double, integer, or string will be used. In this case, it is expected that only one of {boolean, double, integer, or string} will be specified. |
| [SetValue(const Aspose::Cells::Object\& value)](./setvalue/) | Non-integer numeric value,Integer value,String value or Boolean value to use as the query parameter. Used only when parameterType is value. |
| [~ConnectionParameter()](./~connectionparameter/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Namespace [Aspose::Cells::ExternalConnections](../)
* Library [Aspose.Cells for C++](../../)
