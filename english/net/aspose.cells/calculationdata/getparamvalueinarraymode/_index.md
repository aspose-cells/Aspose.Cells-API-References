---
title: CalculationData.GetParamValueInArrayMode
second_title: Aspose.Cells for .NET API Reference
description: CalculationData method. Gets the values of the parameter at given index. If the parameter is some kind of expression that needs to be calculated then it will be calculated in array mode
type: docs
url: /net/aspose.cells/calculationdata/getparamvalueinarraymode/
---
## CalculationData.GetParamValueInArrayMode method

Gets the value(s) of the parameter at given index. If the parameter is some kind of expression that needs to be calculated, then it will be calculated in array mode.

```csharp
public object[][] GetParamValueInArrayMode(int index, int maxRowCount, int maxColumnCount)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The index of the parameter(0 based) |
| maxRowCount | Int32 | The row count limit for the returned array. If it is non-positive or greater than the actual row count, then actual row count will be used. |
| maxColumnCount | Int32 | The column count limit for the returned array. If it is non-positive or greater than the actual row count, then actual column count will be used. |

### Return Value

An array which contains all items represented by the specified parameter.

### Remarks

For an expression that needs to be calculated, taking A:A+B:B as an example: In value mode it will be calculated to a single value according to current cell base. But in array mode, all values of A1+B1,A2+B2,A3+B3,... will be calculated and used to construct the returned array. And for such kind of situation, it is better to specify the limit for the row/column count (such as according to [`MaxDataRow`](../../cells/maxdatarow/) and [`MaxDataColumn`](../../cells/maxdatacolumn/)), otherwise the returned large array may increase memory cost with large amount of useless data.

### Examples

```csharp
// Called: object[][] vs = data.GetParamValueInArrayMode(0, 3, 3);
public override void Method_Int32_(CalculationData data)
            {
                if (_autoMode || _arrayMode)
                {
                    double v = 0.0;
                    object[][] vs = data.GetParamValueInArrayMode(0, 3, 3);
                    for (int i = 0; i < vs.Length; i++)
                    {
                        object[] r = vs[i];
                        for (int j = 0; j < r.Length; j++)
                        {
                            v += (double)r[j];
                        }
                    }
                    if (_autoMode)
                    {
                        object o = data.GetParamValue(1);
                        if (!(o is double))
                        {
                            data.CalculatedValue = "#VALUE!";
                            return;
                        }
                        v += (double)o;
                        o = data.GetParamValue(2);
                        if (!(o is object[][]))
                        {
                            data.CalculatedValue = "#VALUE!";
                            return;
                        }
                        vs = (object[][])o;
                        for (int i = 0; i < vs.Length; i++)
                        {
                            object[] r = vs[i];
                            for (int j = 0; j < r.Length; j++)
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


