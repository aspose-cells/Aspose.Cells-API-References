---
title: Aspose::Cells::AbstractCalculationEngine::ForceRecalculate method
linktitle: ForceRecalculate
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::AbstractCalculationEngine::ForceRecalculate method. Whether to force the given function to be recalculated always when calculating shared formulas in C++.'
type: docs
weight: 600
url: /cpp/aspose.cells/abstractcalculationengine/forcerecalculate/
---
## AbstractCalculationEngine::ForceRecalculate method


Whether to force the given function to be recalculated always when calculating shared formulas.

```cpp
virtual bool Aspose::Cells::AbstractCalculationEngine::ForceRecalculate(const U16String &functionName)
```


| Parameter | Type | Description |
| --- | --- | --- |
| functionName | const U16String\& | name of the function. Generally it is custom function's name. If ProcessBuiltInFunctions is true, then built-in functions will also be checked here. |

## ReturnValue

true if the specified function needs to be recalculated always.
## Remarks



For shared formulas, multiple cells share the same function. If the function's parameters keep same for those cells too, then generally this function needs to be calculated only once. So for performance consideration we only calculate such kind of function once too(Calculate(CalculationData) is called only once, instead of being called repeatedly for every cell). However, for user's custom implementation, maybe the function, especially the custom function, needs to be calculated differently for different cells. If so, user needs to override this method to make it return true for the function. And for Calculate(CalculationData), the given CalculationData.CalculatedValue may have been initialized with the cached value of previous calculation. 
## See Also

* Class [U16String](../../u16string/)
* Class [AbstractCalculationEngine](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
