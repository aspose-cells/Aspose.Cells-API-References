---
title: ConnectionParameter
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 10
url: /python-net/aspose.cells.externalconnections/connectionparameter/
---

## ConnectionParameter class

Specifies properties about any parameters used with external data connections<br/>            Parameters are valid for ODBC and web queries.

The ConnectionParameter type exposes the following members:
## Properties
| Name | Description |
| :- | :- |
|sql_type|SQL data type of the parameter. Only valid for ODBC sources.|
|refresh_on_change|Flag indicating whether the query should automatically refresh when the contents of a <br/>            cell that provides the parameter value changes. If true, then external data is refreshed <br/>            using the new parameter value every time there's a change. If false, then external data <br/>            is only refreshed when requested by the user, or some other event triggers refresh (e.g., workbook opened).|
|prompt|Prompt string for the parameter. Presented to the spreadsheet user along with input UI <br/>            to collect the parameter value before refreshing the external data. Used only when <br/>            parameterType = prompt.|
|type|Type of parameter used.<br/>            If the parameterType=value, then the value from boolean, double, integer, <br/>            or string will be used.  In this case, it is expected that only one of <br/>            {boolean, double, integer, or string} will be specified.|
|name|The name of the parameter.|
|cell_reference|Cell reference indicating which cell's value to use for the query parameter. Used only when parameterType is cell.|
|value|Non-integer numeric value,Integer value,String value or Boolean value<br/>            to use as the query parameter. Used only when parameterType is value.|

### See Also

* namespace [aspose.cells.externalconnections](/cells/python-net/aspose.cells.externalconnections/)
* assembly [Aspose.Cells](/cells/python-net/)

