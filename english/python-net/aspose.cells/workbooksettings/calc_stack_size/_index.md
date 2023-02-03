---
title: calc_stack_size property
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 100
url: /python-net/aspose.cells/workbooksettings/calc_stack_size/
is_root: false
---

## calc_stack_size property


Specifies the stack size for calculating cells recursively.
The large value for this size will give better performance when there are lots of cells need to be calculated recursively.
On the other hand, larger value will raise the risk of StackOverflowException.
If user gets StackOverflowException when calculating formulas, this value should be decreased.

### Remarks 


NOTE: This member is now obsolete. Instead, please use CalculationOptions
with the specified CalcStackSize when calculating formulas.
This property will be removed 12 months later since February 2022. 
Aspose apologizes for any inconvenience you may have experienced.

### See Also
* module [aspose.cells](../../)
* class [WorkbookSettings](/cells/python-net/aspose.cells/workbooksettings)
