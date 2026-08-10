---
title: "ConnectionParameter Class"
linktitle: "ConnectionParameter"
articleTitle: "ConnectionParameter"
second_title: "Aspose.Cells for Python via Java"
description: "Specifies properties about any parameters used with external data connections Parameters are valid for ODBC and web queries."
type: docs
weight: 1150
url: /python-java/asposecells.api/connectionparameter/
---

## ConnectionParameter class

Specifies properties about any parameters used with external data connections Parameters are valid for ODBC and web queries.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [SqlType](#sqltype) | int | SQL data type of the parameter. Only valid for ODBC sources. The value of the property is SqlDataType integer constant. |
| [RefreshOnChange](#refreshonchange) | boolean | Flag indicating whether the query should automatically refresh when the contents of a cell that provides the parameter v |
| [Prompt](#prompt) | String | Prompt string for the parameter. Presented to the spreadsheet user along with input UI to collect the parameter value be |
| [Type](#type) | ConnectionParameterType | Type of parameter used. If the parameterType=value, then the value from boolean, double, integer, or string will be used |
| [Name](#name) | String | The name of the parameter. |
| [CellReference](#cellreference) | String | Cell reference indicating which cell's value to use for the query parameter. Used only when parameterType is cell. |
| [Value](#value) | Object | Non-integer numeric value,Integer value,String value or Boolean value to use as the query parameter. Used only when para |

### ConnectionParameter.SqlType property {#sqltype}

SQL data type of the parameter. Only valid for ODBC sources. The value of the property is SqlDataType integer constant.

**Type:** int

### ConnectionParameter.RefreshOnChange property {#refreshonchange}

Flag indicating whether the query should automatically refresh when the contents of a cell that provides the parameter value changes. If true, then external data is refreshed using the new parameter value every time there's a change. If false, then external data is only refreshed when requested by the user, or some other event triggers refresh (e.g., workbook opened).

**Type:** boolean

### ConnectionParameter.Prompt property {#prompt}

Prompt string for the parameter. Presented to the spreadsheet user along with input UI to collect the parameter value before refreshing the external data. Used only when parameterType = prompt.

**Type:** String

### ConnectionParameter.Type property {#type}

Type of parameter used. If the parameterType=value, then the value from boolean, double, integer, or string will be used. In this case, it is expected that only one of {boolean, double, integer, or string} will be specified.

**Type:** ConnectionParameterType

### ConnectionParameter.Name property {#name}

The name of the parameter.

**Type:** String

### ConnectionParameter.CellReference property {#cellreference}

Cell reference indicating which cell's value to use for the query parameter. Used only when parameterType is cell.

**Type:** String

### ConnectionParameter.Value property {#value}

Non-integer numeric value,Integer value,String value or Boolean value to use as the query parameter. Used only when parameterType is value.

**Type:** Object
