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

If it is some kind of expression that needs to be calculated, then it will be calculated in value mode and generally a single value will be returned according to current cell base. For example, if one parameter of D2's formula is A:A+B:B, then A2+B2 will be calculated and returned. However, if this parameter has been specified as array mode (by [`UpdateCustomFunctionDefinition`](../../workbook/updatecustomfunctiondefinition/) or [`CustomFunctionDefinition`](../../formulaparseoptions/customfunctiondefinition/)), then an array(object[][]) will be returned whose items are A1+B1,A2+B2,....

### Examples

```csharp
// Called: object paramValue = data.GetParamValue(i);
public override void Method_Int32_(CalculationData data)
        {
            // Custom calculation logic
            string funcName = data.FunctionName.ToUpper();
            if (funcName == "MYFUNC")
            {
                // Example custom function logic
                int count = data.ParamCount;
                object result = null;
                for (int i = 0; i < count; i++)
                {
                    object paramValue = data.GetParamValue(i);
                    if (paramValue is ReferredArea)
                    {
                        ReferredArea ra = (ReferredArea)paramValue;
                        paramValue = ra.GetValue(0, 0);
                    }
                    // Process the parameter here
                    // result = ...;
                }
                data.CalculatedValue = result;
            }
        }
```

### See Also

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


