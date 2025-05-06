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
// Called: data.CalculatedValue = data.GetParamValue(0);
public override void Method_Int32_(CalculationData data)
            {
                if (_autoMode || _arrayMode)
                {
                    double v = 0.0;
                    object[][] vs = data.GetParamValueInArrayMode(0, 3, 3);
                    for (int i = 0; i &lt; vs.Length; i++)
                    {
                        object[] r = vs[i];
                        for (int j = 0; j &lt; r.Length; j++)
                        {
                            v += (double)r[j];
                        }
                    }
                    if (_autoMode)
                    {
                        object o = data.GetParamValue(1);
                        if (!(o is double))
                        {
                            data.CalculatedValue = &quot;#VALUE!&quot;;
                            return;
                        }
                        v += (double)o;
                        o = data.GetParamValue(2);
                        if (!(o is object[][]))
                        {
                            data.CalculatedValue = &quot;#VALUE!&quot;;
                            return;
                        }
                        vs = (object[][])o;
                        for (int i = 0; i &lt; vs.Length; i++)
                        {
                            object[] r = vs[i];
                            for (int j = 0; j &lt; r.Length; j++)
                            {
                                v += (double)r[j];
                            }
                        }
                    }
                    data.CalculatedValue = v;
                }
                else
                {
                    data.CalculatedValue = data.GetParamValue(0);
                }
            }
```

### See Also

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


