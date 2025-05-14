---
title: CalculationData.FunctionName
second_title: Aspose.Cells for .NET API Reference
description: CalculationData property. Gets the function name to be calculated
type: docs
url: /net/aspose.cells/calculationdata/functionname/
---
## CalculationData.FunctionName property

Gets the function name to be calculated.

```csharp
public string FunctionName { get; }
```

### Examples

```csharp
// Called: if (data.FunctionName.ToUpper() == "MYFUNC")
public override void CalculationData_Property_FunctionName(CalculationData data)
        {
            // Example: Custom implementation for a function named "MYFUNC"
            if (data.FunctionName.ToUpper() == "MYFUNC")
            {
                // Assuming MYFUNC takes two parameters and returns their sum
                Aspose.Cells.ReferredArea paramArea1 = (Aspose.Cells.ReferredArea)data.GetParamValue(0);
                Aspose.Cells.ReferredArea paramArea2 = (Aspose.Cells.ReferredArea)data.GetParamValue(1);

                double param1 = Convert.ToDouble(paramArea1.GetValue(0, 0));
                double param2 = Convert.ToDouble(paramArea2.GetValue(0, 0));
                data.CalculatedValue = param1 + param2;
            }
        }
```

### See Also

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


