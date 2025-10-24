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
| [value](#value--)| Object | Non-integer numeric value,Integer value,String value or Boolean value to use as the query parameter. Used only when parameterType is value. |
## Methods
| Method | Description |
| --- | --- |
| [getSqlType()](#getSqlType--)| <b>@deprecated.</b> Please use the 'sqlType' property instead. SQL data type of the parameter. Only valid for ODBC sources. |
| [setSqlType(SqlDataType)](#setSqlType-sqldatatype-)| <b>@deprecated.</b> Please use the 'sqlType' property instead. SQL data type of the parameter. Only valid for ODBC sources. |
| [getRefreshOnChange()](#getRefreshOnChange--)| <b>@deprecated.</b> Please use the 'refreshOnChange' property instead. Flag indicating whether the query should automatically refresh when the contents of a cell that provides the parameter value changes. If true, then external data is refreshed using the new parameter value every time there's a change. If false, then external data is only refreshed when requested by the user, or some other event triggers refresh (e.g., workbook opened). |
| [setRefreshOnChange(boolean)](#setRefreshOnChange-boolean-)| <b>@deprecated.</b> Please use the 'refreshOnChange' property instead. Flag indicating whether the query should automatically refresh when the contents of a cell that provides the parameter value changes. If true, then external data is refreshed using the new parameter value every time there's a change. If false, then external data is only refreshed when requested by the user, or some other event triggers refresh (e.g., workbook opened). |
| [getPrompt()](#getPrompt--)| <b>@deprecated.</b> Please use the 'prompt' property instead. Prompt string for the parameter. Presented to the spreadsheet user along with input UI to collect the parameter value before refreshing the external data. Used only when parameterType = prompt. |
| [setPrompt(string)](#setPrompt-string-)| <b>@deprecated.</b> Please use the 'prompt' property instead. Prompt string for the parameter. Presented to the spreadsheet user along with input UI to collect the parameter value before refreshing the external data. Used only when parameterType = prompt. |
| [getType()](#getType--)| <b>@deprecated.</b> Please use the 'type' property instead. Type of parameter used. If the parameterType=value, then the value from boolean, double, integer, or string will be used.  In this case, it is expected that only one of {boolean, double, integer, or string} will be specified. |
| [setType(ConnectionParameterType)](#setType-connectionparametertype-)| <b>@deprecated.</b> Please use the 'type' property instead. Type of parameter used. If the parameterType=value, then the value from boolean, double, integer, or string will be used.  In this case, it is expected that only one of {boolean, double, integer, or string} will be specified. |
| [getName()](#getName--)| <b>@deprecated.</b> Please use the 'name' property instead. The name of the parameter. |
| [setName(string)](#setName-string-)| <b>@deprecated.</b> Please use the 'name' property instead. The name of the parameter. |
| [getCellReference()](#getCellReference--)| <b>@deprecated.</b> Please use the 'cellReference' property instead. Cell reference indicating which cell's value to use for the query parameter. Used only when parameterType is cell. |
| [setCellReference(string)](#setCellReference-string-)| <b>@deprecated.</b> Please use the 'cellReference' property instead. Cell reference indicating which cell's value to use for the query parameter. Used only when parameterType is cell. |
| [getValue()](#getValue--)| <b>@deprecated.</b> Please use the 'value' property instead. Non-integer numeric value,Integer value,String value or Boolean value to use as the query parameter. Used only when parameterType is value. |
| [setValue(Object)](#setValue-object-)| <b>@deprecated.</b> Please use the 'value' property instead. Non-integer numeric value,Integer value,String value or Boolean value to use as the query parameter. Used only when parameterType is value. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
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
value : Object;
```
### getSqlType() {#getSqlType--}
```javascript
getSqlType() : SqlDataType;
```
**Returns**
[SqlDataType](../sqldatatype/)
### setSqlType(SqlDataType) {#setSqlType-sqldatatype-}
```javascript
setSqlType(value: SqlDataType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SqlDataType](../sqldatatype/) | The value to set. |
### getRefreshOnChange() {#getRefreshOnChange--}
```javascript
getRefreshOnChange() : boolean;
```
### setRefreshOnChange(boolean) {#setRefreshOnChange-boolean-}
```javascript
setRefreshOnChange(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getPrompt() {#getPrompt--}
```javascript
getPrompt() : string;
```
### setPrompt(string) {#setPrompt-string-}
```javascript
setPrompt(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getType() {#getType--}
```javascript
getType() : ConnectionParameterType;
```
**Returns**
[ConnectionParameterType](../connectionparametertype/)
### setType(ConnectionParameterType) {#setType-connectionparametertype-}
```javascript
setType(value: ConnectionParameterType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ConnectionParameterType](../connectionparametertype/) | The value to set. |
### getName() {#getName--}
```javascript
getName() : string;
```
### setName(string) {#setName-string-}
```javascript
setName(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getCellReference() {#getCellReference--}
```javascript
getCellReference() : string;
```
### setCellReference(string) {#setCellReference-string-}
```javascript
setCellReference(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getValue() {#getValue--}
```javascript
getValue() : Object;
```
### setValue(Object) {#setValue-object-}
```javascript
setValue(value: Object) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Object | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
