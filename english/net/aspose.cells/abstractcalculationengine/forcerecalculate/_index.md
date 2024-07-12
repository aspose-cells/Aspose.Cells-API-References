---
title: AbstractCalculationEngine.ForceRecalculate
second_title: Aspose.Cells for .NET API Reference
description: AbstractCalculationEngine method. Whether force given function to be recalculated always when calculating shared formulas
type: docs
url: /net/aspose.cells/abstractcalculationengine/forcerecalculate/
---
## AbstractCalculationEngine.ForceRecalculate method

Whether force given function to be recalculated always when calculating shared formulas.

```csharp
public virtual bool ForceRecalculate(string functionName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| functionName | String | name of the function. Generally it is custom function's name. If [`ProcessBuiltInFunctions`](../processbuiltinfunctions/) is true, then built-in functions will also be checked here. |

### Return Value

true if the specified function needs to be recalculated always.

### Remarks

For shared formulas, multiple cells share the same function. If the function's parameters keep same for those cells too, then generally this function needs to be calculated only once. So for performance consideration we only calculate such kind of function once too([`Calculate`](../calculate/) is called only once, instead of being called repeatedly for every cell). However, for user's custom implementation, maybe the function, especially the custom function, needs to be calculated differently for different cells. If so, user needs to override this method to make it return true for the function. And for [`Calculate`](../calculate/), the given [`CalculatedValue`](../../calculationdata/calculatedvalue/) may have been initialized with the cached value of previous calculation.

### See Also

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


