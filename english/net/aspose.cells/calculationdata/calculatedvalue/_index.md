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

User should set this property in his custom calculation engine for those functions the engine supports, and the set value will be returned when getting this property later. The set value may be of possible types of !:Cell.Value, or array of such kind of values, or a Range, Name, ReferredArea. Getting this property before setting value to it will make the function be calculated by the default calculation engine of Aspose.Cells and then the calculated value will be returned(generally it should be #NAME? for user-defined functions).

### See Also

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


