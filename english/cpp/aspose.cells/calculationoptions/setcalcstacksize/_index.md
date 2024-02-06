﻿---
title: Aspose::Cells::CalculationOptions::SetCalcStackSize method
linktitle: SetCalcStackSize
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::CalculationOptions::SetCalcStackSize method. The stack size for calculating cells recursively. Default value is 200 in C++.'
type: docs
weight: 1300
url: /cpp/aspose.cells/calculationoptions/setcalcstacksize/
---
## CalculationOptions::SetCalcStackSize method


The stack size for calculating cells recursively. Default value is 200.

```cpp
void Aspose::Cells::CalculationOptions::SetCalcStackSize(int32_t value)
```

## Remarks


When there are large amount of cells need to be calculated recursively in the dependency tree, StackOverflowException may be caused in the calculation process. If so, user should specify smaller value for this property. For such situation, user should determine the proper value for this property according to the actual formulas and data. However, too small value may cause performance degradation for the formula calculation and value less than 2 will make it impossible to calculate formula which depends on another one. So if the specified value is less than 2, it will be reset to 2. 
## See Also

* Class [CalculationOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
