---
title: CalculationData.GetParamValue
second_title: Aspose.Cells for .NET API Reference
description: CalculationData method. Gets the represented value object of the parameter at given index
type: docs
url: /net/aspose.cells/calculationdata/getparamvalue/
---
## CalculationData.GetParamValue method

Gets the represented value object of the parameter at given index.

```csharp
public object GetParamValue(int index)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The index of the parameter(0 based) |

### Return Value

The calculated value of the parameter.

### Remarks

For one parameter:

If it is plain value, then returns the plain value itself;

If it is reference, then returns ReferredArea object;

If it references to dataset(s) with multiple values, then returns array of objects;

If it is some kind of expression that needs to be calculated, then it will be calculated in value mode and generally a single value will be returned according to current cell base. For example, if one parameter of D2's formula is A:A+B:B, then A2+B2 will be calculated and returned. However, if this parameter has been specified as array mode (by !:Workbook.UpdateCustomFunctionDefinition(CustomFunctionDefinition) or [`CustomFunctionDefinition`](../../formulaparseoptions/customfunctiondefinition/)), then an array(object[][]) will be returned whose items are A1+B1,A2+B2,....

### See Also

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


