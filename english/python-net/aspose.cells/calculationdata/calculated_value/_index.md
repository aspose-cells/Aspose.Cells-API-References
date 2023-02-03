---
title: calculated_value property
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 50
url: /python-net/aspose.cells/calculationdata/calculated_value/
is_root: false
---

## calculated_value property


Gets or sets the calculated value for this function.

### Remarks 


User should set this property in his custom calculation engine for those functions the engine supports,
and the set value will be returned when getting this property later.
The set value can be any value of those objects that can be set to a Cell(Cell.Value).
And it can also be array of such kind of values, or a Range, Name, ReferredArea.
Getting this property before setting will make the function be calculated by the default calculation engine of Aspose.Cells and the calculated value will be returned.

### See Also
* module [aspose.cells](../../)
* class [CalculationData](/cells/python-net/aspose.cells/calculationdata)
