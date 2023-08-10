---
title: AbstractCalculationEngine.IsParamArrayModeRequired
second_title: Aspose.Cells for .NET API Reference
description: AbstractCalculationEngine property. Indicates whether this engine needs the parameter to be calculated in array mode. Default value is false. If GetParamValueInArrayMode is required when calculating custom functions this property needs to be set as true
type: docs
url: /net/aspose.cells/abstractcalculationengine/isparamarraymoderequired/
---
## AbstractCalculationEngine.IsParamArrayModeRequired property

Indicates whether this engine needs the parameter to be calculated in array mode. Default value is false. If [`GetParamValueInArrayMode`](../../calculationdata/getparamvalueinarraymode/) is required when calculating custom functions, this property needs to be set as true.

```csharp
public virtual bool IsParamArrayModeRequired { get; }
```

### Remarks

If this custom calculation engine needs the parameter to be calculated in array mode, more stacks will be required to cache the tree for parameters and Calculate() method may be called recursively to calculate the parameter's value. For performance consideration, if no special requirement, please keep this property as the default value(false).

### See Also

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


