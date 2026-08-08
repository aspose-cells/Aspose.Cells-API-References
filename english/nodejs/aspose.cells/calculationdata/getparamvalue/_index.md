---
title: "CalculationData.getParamValue"
linktitle: "getParamValue"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Gets the represented value object of the parameter at given index."
type: docs
weight: 80
url: /nodejs/aspose.cells/calculationdata/getparamvalue/
---

## getParamValue(index)

Gets the represented value object of the parameter at given index. For one parameter: If it is plain value, then returns the plain value itself;If it is reference, then returns ReferredArea object;If it references to dataset(s) with multiple values, then returns array of objects; If it is some kind of expression that needs to be calculated, then it will be calculated in value mode and generally a single value will be returned according to current cell base. For example, if one parameter of D2's formula is A:A+B:B, then A2+B2 will be calculated and returned. However, if this parameter has been specified as array mode (by Workbook.updateCustomFunctionDefinition(com.aspose.cells.CustomFunctionDefinition) or FormulaParseOptions.CustomFunctionDefinition), then an array(object[][]) will be returned whose items are A1+B1,A2+B2,....

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The index of the parameter(0 based) |

**Returns:** Object — `Object` The calculated value of the parameter.
