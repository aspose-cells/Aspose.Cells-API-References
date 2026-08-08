---
title: "ConnectionParameter"
linktitle: "ConnectionParameter"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Specifies properties about any parameters used with external data connections Parameters are valid for ODBC and web queries."
type: docs
weight: 820
url: /nodejs/aspose.cells/connectionparameter/
---

## ConnectionParameter class

Specifies properties about any parameters used with external data connections Parameters are valid for ODBC and web queries.

## Methods

| Name | Description |
| --- | --- |
| [getCellReference()](#getcellreference) | Cell reference indicating which cell's value to use for the query parameter. Used only when parameterType is cell. |
| [getName()](#getname) | The name of the parameter. |
| [getPrompt()](#getprompt) | Prompt string for the parameter. Presented to the spreadsheet user along with input UI to collect the parameter value be |
| [getRefreshOnChange()](#getrefreshonchange) | Flag indicating whether the query should automatically refresh when the contents of a cell that provides the parameter v |
| [getSqlType()](#getsqltype) | SQL data type of the parameter. Only valid for ODBC sources. The value of the property is SqlDataType integer constant. |
| [getType()](#gettype) | Type of parameter used. If the parameterType=value, then the value from boolean, double, integer, or string will be used |
| [getValue()](#getvalue) | Non-integer numeric value,Integer value,String value or Boolean value to use as the query parameter. Used only when para |
| [setCellReference()](#setcellreference) | Cell reference indicating which cell's value to use for the query parameter. Used only when parameterType is cell. |
| [setName()](#setname) | The name of the parameter. |
| [setPrompt()](#setprompt) | Prompt string for the parameter. Presented to the spreadsheet user along with input UI to collect the parameter value be |
| [setRefreshOnChange()](#setrefreshonchange) | Flag indicating whether the query should automatically refresh when the contents of a cell that provides the parameter v |
| [setSqlType()](#setsqltype) | SQL data type of the parameter. Only valid for ODBC sources. The value of the property is SqlDataType integer constant. |
| [setValue()](#setvalue) | Non-integer numeric value,Integer value,String value or Boolean value to use as the query parameter. Used only when para |

### getCellReference() {#getcellreference}

Cell reference indicating which cell's value to use for the query parameter. Used only when parameterType is cell.

### getName() {#getname}

The name of the parameter.

### getPrompt() {#getprompt}

Prompt string for the parameter. Presented to the spreadsheet user along with input UI to collect the parameter value before refreshing the external data. Used only when parameterType = prompt.

### getRefreshOnChange() {#getrefreshonchange}

Flag indicating whether the query should automatically refresh when the contents of a cell that provides the parameter value changes. If true, then external data is refreshed using the new parameter value every time there's a change. If false, then external data is only refreshed when requested by the user, or some other event triggers refresh (e.g., workbook opened).

### getSqlType() {#getsqltype}

SQL data type of the parameter. Only valid for ODBC sources. The value of the property is SqlDataType integer constant.

### getType() {#gettype}

Type of parameter used. If the parameterType=value, then the value from boolean, double, integer, or string will be used. In this case, it is expected that only one of {boolean, double, integer, or string} will be specified.

### getValue() {#getvalue}

Non-integer numeric value,Integer value,String value or Boolean value to use as the query parameter. Used only when parameterType is value.

### setCellReference() {#setcellreference}

Cell reference indicating which cell's value to use for the query parameter. Used only when parameterType is cell.

### setName() {#setname}

The name of the parameter.

### setPrompt() {#setprompt}

Prompt string for the parameter. Presented to the spreadsheet user along with input UI to collect the parameter value before refreshing the external data. Used only when parameterType = prompt.

### setRefreshOnChange() {#setrefreshonchange}

Flag indicating whether the query should automatically refresh when the contents of a cell that provides the parameter value changes. If true, then external data is refreshed using the new parameter value every time there's a change. If false, then external data is only refreshed when requested by the user, or some other event triggers refresh (e.g., workbook opened).

### setSqlType() {#setsqltype}

SQL data type of the parameter. Only valid for ODBC sources. The value of the property is SqlDataType integer constant.

### setValue() {#setvalue}

Non-integer numeric value,Integer value,String value or Boolean value to use as the query parameter. Used only when parameterType is value.
