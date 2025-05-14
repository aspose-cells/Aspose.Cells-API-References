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
// Called: data.CalculatedValue = "Success";
public override void CalculationData_Property_CalculatedValue(CalculationData data)
            {
                object p = data.GetParamValue(0);
                if (p is ReferredArea)
                {
                    if (_copts != null && _copts.Recursive)
                    {
                        _copts.Recursive = false;
                        try
                        {
                            ProcessReference((ReferredArea)p);
                        }
                        finally
                        {
                            _copts.Recursive = true;
                        }
                    }
                    else
                    {
                        ProcessReference((ReferredArea)p);
                    }
                }
                data.CalculatedValue = "Success";
            }
```

### See Also

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


