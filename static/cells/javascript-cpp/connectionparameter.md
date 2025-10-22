##ConnectionParameter
Specifies properties about any parameters used with external data connections Parameters are valid for ODBC and web queries.
## ConnectionParameter class
Specifies properties about any parameters used with external data connections Parameters are valid for ODBC and web queries.
```javascript
class ConnectionParameter;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [sqlType](#sqlType--)| SqlDataType | SQL data type of the parameter. Only valid for ODBC sources. |
| [refreshOnChange](#refreshOnChange--)| boolean | Flag indicating whether the query should automatically refresh when the contents of a cell that provides the parameter value changes. If true, then external data is refreshed using the new parameter value every time there's a change. If false, then external data is only refreshed when requested by the user, or some other event triggers refresh (e.g., workbook opened). |
| [prompt](#prompt--)| string | Prompt string for the parameter. Presented to the spreadsheet user along with input UI to collect the parameter value before refreshing the external data. Used only when parameterType = prompt. |
| [type](#type--)| ConnectionParameterType | Type of parameter used. If the parameterType=value, then the value from boolean, double, integer, or string will be used.  In this case, it is expected that only one of {boolean, double, integer, or string} will be specified. |
| [name](#name--)| string | The name of the parameter. |
| [cellReference](#cellReference--)| string | Cell reference indicating which cell's value to use for the query parameter. Used only when parameterType is cell. |
| [value](#value--)| VObject | Non-integer numeric value,Integer value,String value or Boolean value to use as the query parameter. Used only when parameterType is value. |
### sqlType {#sqlType--}
SQL data type of the parameter. Only valid for ODBC sources.
```javascript
sqlType : SqlDataType;
```
### refreshOnChange {#refreshOnChange--}
Flag indicating whether the query should automatically refresh when the contents of a cell that provides the parameter value changes. If true, then external data is refreshed using the new parameter value every time there's a change. If false, then external data is only refreshed when requested by the user, or some other event triggers refresh (e.g., workbook opened).
```javascript
refreshOnChange : boolean;
```
### prompt {#prompt--}
Prompt string for the parameter. Presented to the spreadsheet user along with input UI to collect the parameter value before refreshing the external data. Used only when parameterType = prompt.
```javascript
prompt : string;
```
### type {#type--}
Type of parameter used. If the parameterType=value, then the value from boolean, double, integer, or string will be used.  In this case, it is expected that only one of {boolean, double, integer, or string} will be specified.
```javascript
type : ConnectionParameterType;
```
### name {#name--}
The name of the parameter.
```javascript
name : string;
```
### cellReference {#cellReference--}
Cell reference indicating which cell's value to use for the query parameter. Used only when parameterType is cell.
```javascript
cellReference : string;
```
### value {#value--}
Non-integer numeric value,Integer value,String value or Boolean value to use as the query parameter. Used only when parameterType is value.
```javascript
value : VObject;
```
