---
title: ConnectionParameter
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Specifies properties about any parameters used with external data connections Parameters are valid for ODBC and web queries.
type: docs
url: /nodejs-cpp/connectionparameter/
---

## ConnectionParameter class

Specifies properties about any parameters used with external data connections Parameters are valid for ODBC and web queries.

```javascript
class ConnectionParameter;
```


## Methods

| Method | Description |
| --- | --- |
| [getSqlType()](#getSqlType--)| SQL data type of the parameter. Only valid for ODBC sources. |
| [setSqlType(SqlDataType)](#setSqlType-sqldatatype-)| SQL data type of the parameter. Only valid for ODBC sources. |
| [getRefreshOnChange()](#getRefreshOnChange--)| Flag indicating whether the query should automatically refresh when the contents of a cell that provides the parameter value changes. If true, then external data is refreshed using the new parameter value every time there's a change. If false, then external data is only refreshed when requested by the user, or some other event triggers refresh (e.g., workbook opened). |
| [setRefreshOnChange(boolean)](#setRefreshOnChange-boolean-)| Flag indicating whether the query should automatically refresh when the contents of a cell that provides the parameter value changes. If true, then external data is refreshed using the new parameter value every time there's a change. If false, then external data is only refreshed when requested by the user, or some other event triggers refresh (e.g., workbook opened). |
| [getPrompt()](#getPrompt--)| Prompt string for the parameter. Presented to the spreadsheet user along with input UI to collect the parameter value before refreshing the external data. Used only when parameterType = prompt. |
| [setPrompt(string)](#setPrompt-string-)| Prompt string for the parameter. Presented to the spreadsheet user along with input UI to collect the parameter value before refreshing the external data. Used only when parameterType = prompt. |
| [getType()](#getType--)| Type of parameter used. If the parameterType=value, then the value from boolean, double, integer, or string will be used.  In this case, it is expected that only one of {boolean, double, integer, or string} will be specified. |
| [setType(ConnectionParameterType)](#setType-connectionparametertype-)| Type of parameter used. If the parameterType=value, then the value from boolean, double, integer, or string will be used.  In this case, it is expected that only one of {boolean, double, integer, or string} will be specified. |
| [getName()](#getName--)| The name of the parameter. |
| [setName(string)](#setName-string-)| The name of the parameter. |
| [getCellReference()](#getCellReference--)| Cell reference indicating which cell's value to use for the query parameter. Used only when parameterType is cell. |
| [setCellReference(string)](#setCellReference-string-)| Cell reference indicating which cell's value to use for the query parameter. Used only when parameterType is cell. |


### getSqlType() {#getSqlType--}

SQL data type of the parameter. Only valid for ODBC sources.

```javascript
getSqlType() : SqlDataType;
```


**Returns**

[SqlDataType](/nodejs-cpp/sqldatatype/)

### setSqlType(SqlDataType) {#setSqlType-sqldatatype-}

SQL data type of the parameter. Only valid for ODBC sources.

```javascript
setSqlType(value: SqlDataType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SqlDataType](/nodejs-cpp/sqldatatype/) | The value to set. |

### getRefreshOnChange() {#getRefreshOnChange--}

Flag indicating whether the query should automatically refresh when the contents of a cell that provides the parameter value changes. If true, then external data is refreshed using the new parameter value every time there's a change. If false, then external data is only refreshed when requested by the user, or some other event triggers refresh (e.g., workbook opened).

```javascript
getRefreshOnChange() : boolean;
```


### setRefreshOnChange(boolean) {#setRefreshOnChange-boolean-}

Flag indicating whether the query should automatically refresh when the contents of a cell that provides the parameter value changes. If true, then external data is refreshed using the new parameter value every time there's a change. If false, then external data is only refreshed when requested by the user, or some other event triggers refresh (e.g., workbook opened).

```javascript
setRefreshOnChange(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getPrompt() {#getPrompt--}

Prompt string for the parameter. Presented to the spreadsheet user along with input UI to collect the parameter value before refreshing the external data. Used only when parameterType = prompt.

```javascript
getPrompt() : string;
```


### setPrompt(string) {#setPrompt-string-}

Prompt string for the parameter. Presented to the spreadsheet user along with input UI to collect the parameter value before refreshing the external data. Used only when parameterType = prompt.

```javascript
setPrompt(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getType() {#getType--}

Type of parameter used. If the parameterType=value, then the value from boolean, double, integer, or string will be used.  In this case, it is expected that only one of {boolean, double, integer, or string} will be specified.

```javascript
getType() : ConnectionParameterType;
```


**Returns**

[ConnectionParameterType](/nodejs-cpp/connectionparametertype/)

### setType(ConnectionParameterType) {#setType-connectionparametertype-}

Type of parameter used. If the parameterType=value, then the value from boolean, double, integer, or string will be used.  In this case, it is expected that only one of {boolean, double, integer, or string} will be specified.

```javascript
setType(value: ConnectionParameterType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ConnectionParameterType](/nodejs-cpp/connectionparametertype/) | The value to set. |

### getName() {#getName--}

The name of the parameter.

```javascript
getName() : string;
```


### setName(string) {#setName-string-}

The name of the parameter.

```javascript
setName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getCellReference() {#getCellReference--}

Cell reference indicating which cell's value to use for the query parameter. Used only when parameterType is cell.

```javascript
getCellReference() : string;
```


### setCellReference(string) {#setCellReference-string-}

Cell reference indicating which cell's value to use for the query parameter. Used only when parameterType is cell.

```javascript
setCellReference(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |


