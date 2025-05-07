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
// Called: data.CalculatedValue = data.GetParamValue(0);
public override void Property_CalculatedValue(CalculationData data)
            {
                if (stage == 0)
                {
                    data.CalculatedValue = 0;
                    return;
                }
                string s = data.FunctionName.ToLower();
                if ("crow".Equals(s))
                {
                    data.CalculatedValue = data.GetParamValue(0);
                }
                else if ("crow2".Equals(s))
                {
                    data.CalculatedValue = data.CellRow + 1;
                }
            }
```

### See Also

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


