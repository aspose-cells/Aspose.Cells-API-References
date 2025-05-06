---
title: CalculationData.CalculatedValue
second_title: Aspose.Cells for .NET API Reference
description: CalculationData property. Gets or sets the calculated value for this function
type: docs
url: /net/aspose.cells/calculationdata/calculatedvalue/
---
## CalculationData.CalculatedValue property

Gets or sets the calculated value for this function.

```csharp
public object CalculatedValue { get; set; }
```

### Remarks

User should set this property in his custom calculation engine for those functions the engine supports, and the set value will be returned when getting this property later. The set value may be of possible types of [`Value`](../../cell/value/), or array of such kind of values, or a Range, Name, ReferredArea. Getting this property before setting value to it will make the function be calculated by the default calculation engine of Aspose.Cells and then the calculated value will be returned(generally it should be #NAME? for user-defined functions).

### Examples

```csharp
// Called: data.CalculatedValue = 0;
public override void Property_CalculatedValue(CalculationData data)
            {
                if (data.FunctionName == &quot;MYSUM&quot;)
                {
                    for (int i = 0; i &lt; data.ParamCount; i++)
                    {
                        object p = data.GetParamValue(i);
                        if (p is Array)
                        {
                            Array array = (Array)p;
                            for (int j = 0; j &lt; array.Length; j++)
                            {
                                object sub = array.GetValue(j);
                                if (sub == null)
                                {
                                    continue;
                                }
                                else if (sub is Array)
                                {
                                    Array subArray = (Array)sub;
                                    for (int k = 0; k &lt; subArray.Length; k++)
                                    {
                                        Assert.IsTrue(sub.ToString().IndexOf(&quot;x&quot;) == -1);
                                    }
                                }
                                else
                                {
                                    Assert.IsTrue(sub.ToString().IndexOf(&quot;x&quot;) == -1);
                                }
                            }
                        }
                    }
                    data.CalculatedValue = 9999;
                    return;
                }
                if (data.FunctionName == &quot;BDP&quot;)
                {
                    data.CalculatedValue = 111;
                    return;
                }
                data.CalculatedValue = 0;
            }
```

### See Also

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


