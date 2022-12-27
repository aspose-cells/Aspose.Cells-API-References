---
title: is_param_literal_required property
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 40
url: /python-net/aspose.cells/abstractcalculationengine/is_param_literal_required/
is_root: false
---

## is_param_literal_required property


Indicates whether this engine needs the literal text of parameter while doing calculation. Default value is false.
### Remarks 


If this custom calculation engine requires the parameter's literal text, more stacks will be required to cache the literal text for parameters and Calculate() method may be called recursively to calculate the parameter's value.
Commonly the literal text is not needed for calculating formulas and this method should return false for most implementations to get better performance.

### See Also
* module [aspose.cells](../../)
* class [AbstractCalculationEngine](/cells/python-net/aspose.cells/abstractcalculationengine)
