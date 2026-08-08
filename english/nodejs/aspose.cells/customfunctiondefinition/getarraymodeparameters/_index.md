---
title: "CustomFunctionDefinition.getArrayModeParameters"
linktitle: "getArrayModeParameters"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Gets the indices of given custom function's parameters that need to be calculated in array mode."
type: docs
weight: 20
url: /nodejs/aspose.cells/customfunctiondefinition/getarraymodeparameters/
---

## getArrayModeParameters(functionName)

Gets the indices of given custom function's parameters that need to be calculated in array mode. For an expression that needs to be calculated, taking A:A+B:B as an example: Generally in value mode it will be calculated to a single value according to current cell base. But in array mode, all values of A1+B1,A2+B2,A3+B3,... will be calculated and used for the calculation.

| Parameter | Type | Description |
| --- | --- | --- |
| functionName | String | Name of the custom function. |

**Returns:** Array of Number — `Array of Number` Indices of the parameters that need to be calculated in array mode for given custom function. Default is null, there is no parameter which needs to be calculated in array mode for the custom function.
