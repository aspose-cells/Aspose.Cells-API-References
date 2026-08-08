---
title: "CalculationData.getParamValueInArrayMode"
linktitle: "getParamValueInArrayMode"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Gets the value(s) of the parameter at given index."
type: docs
weight: 90
url: /nodejs/aspose.cells/calculationdata/getparamvalueinarraymode/
---

## getParamValueInArrayMode(index, maxRowCount, maxColumnCount)

Gets the value(s) of the parameter at given index. If the parameter is some kind of expression that needs to be calculated, then it will be calculated in array mode. For an expression that needs to be calculated, taking A:A+B:B as an example: In value mode it will be calculated to a single value according to current cell base. But in array mode, all values of A1+B1,A2+B2,A3+B3,... will be calculated and used to construct the returned array. And for such kind of situation, it is better to specify the limit for the row/column count (such as according to Cells.MaxDataRow and Cells.MaxDataColumn), otherwise the returned large array may increase memory cost with large amount of useless data.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The index of the parameter(0 based) |
| maxRowCount | Number | The row count limit for the returned array. If it is non-positive or greater than the actual row count, then actual row count will be used. |
| maxColumnCount | Number | The column count limit for the returned array. If it is non-positive or greater than the actual row count, then actual column count will be used. |

**Returns:** Array of Array of Object — `Array of Array of Object` An array which contains all items represented by the specified parameter.
