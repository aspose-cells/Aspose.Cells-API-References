##ConnectionParameter Class
'ConnectionParameter class. Encapsulates the object that represents connectionparameter in Go.'
## ConnectionParameter class
Specifies properties about any parameters used with external data connectionsParameters are valid for ODBC and web queries.
```go
type ConnectionParameter struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetSqlType](./getsqltype/) | SQL data type of the parameter. Only valid for ODBC sources. |
|[SetSqlType](./setsqltype/) | SQL data type of the parameter. Only valid for ODBC sources. |
|[GetRefreshOnChange](./getrefreshonchange/) | Flag indicating whether the query should automatically refresh when the contents of acell that provides the parameter value changes. If true, then external data is refreshedusing the new parameter value every time there's a change. If false, then external datais only refreshed when requested by the user, or some other event triggers refresh (e.g., workbook opened). |
|[SetRefreshOnChange](./setrefreshonchange/) | Flag indicating whether the query should automatically refresh when the contents of acell that provides the parameter value changes. If true, then external data is refreshedusing the new parameter value every time there's a change. If false, then external datais only refreshed when requested by the user, or some other event triggers refresh (e.g., workbook opened). |
|[GetPrompt](./getprompt/) | Prompt string for the parameter. Presented to the spreadsheet user along with input UIto collect the parameter value before refreshing the external data. Used only whenparameterType = prompt. |
|[SetPrompt](./setprompt/) | Prompt string for the parameter. Presented to the spreadsheet user along with input UIto collect the parameter value before refreshing the external data. Used only whenparameterType = prompt. |
|[GetType](./gettype/) | Type of parameter used.If the parameterType=value, then the value from boolean, double, integer,or string will be used.  In this case, it is expected that only one of{boolean, double, integer, or string} will be specified. |
|[SetType](./settype/) | Type of parameter used.If the parameterType=value, then the value from boolean, double, integer,or string will be used.  In this case, it is expected that only one of{boolean, double, integer, or string} will be specified. |
|[GetName](./getname/) | The name of the parameter. |
|[SetName](./setname/) | The name of the parameter. |
|[GetCellReference](./getcellreference/) | Cell reference indicating which cell's value to use for the query parameter. Used only when parameterType is cell. |
|[SetCellReference](./setcellreference/) | Cell reference indicating which cell's value to use for the query parameter. Used only when parameterType is cell. |
|[GetValue](./getvalue/) | Non-integer numeric value,Integer value,String value or Boolean valueto use as the query parameter. Used only when parameterType is value. |
|[SetValue](./setvalue/) | Non-integer numeric value,Integer value,String value or Boolean valueto use as the query parameter. Used only when parameterType is value. |
