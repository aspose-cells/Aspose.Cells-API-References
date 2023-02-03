---
title: calc_stack_size property
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 30
url: /python-net/aspose.cells/calculationoptions/calc_stack_size/
is_root: false
---

## calc_stack_size property


Specifies the stack size for calculating cells recursively.

### Remarks 


When there are large amount of cells need to be calculated recursively in the dependency tree,
StackOverflowException may be caused in the calculation process.
If so, user should specify smaller value for this property.
For such situation, user should determine the proper value for this property according to the actual formulas and data.
Too small value may cause performance degradation for the formula calculation.

### See Also
* module [aspose.cells](../../)
* class [CalculationOptions](/cells/python-net/aspose.cells/calculationoptions)
