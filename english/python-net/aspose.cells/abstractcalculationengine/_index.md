---
title: AbstractCalculationEngine class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 20
url: /python-net/aspose.cells/abstractcalculationengine/
is_root: false
---

## AbstractCalculationEngine class

Represents user's custom calculation engine to extend the default calculation engine of Aspose.Cells.



The AbstractCalculationEngine type exposes the following members:

### Properties
| Property | Description |
| :- | :- |
| [is_param_literal_required](/cells/python-net/aspose.cells/abstractcalculationengine/is_param_literal_required) | Indicates whether this engine needs the literal text of parameter while doing calculation. Default value is false. |
| [process_built_in_functions](/cells/python-net/aspose.cells/abstractcalculationengine/process_built_in_functions) | Whether built-in functions that have been supported by the built-in engine should be checked and processed by this implementation.<br/>Default is false.<br/>If user needs to change the calculation logic of some built-in functions, this property should be set as true. |


### Methods
| Method | Description |
| :- | :- |
| [calculate(data)](/cells/python-net/aspose.cells/abstractcalculationengine/calculate/#CalculationData) | Calculates one function with given data. |


### Remarks 


User should not modify any part of the Workbook directly in this implementation(except the calculated result of the custom function, which can be set by CalculationData.CalculatedValue property).
Otherwise unexpected result or Exception may be caused.
If user needs to change other data than calculated result in the implementation for some custom functions,
for example, change cell's formula, style, ...etc., user should gather those data in this implementation and change them out of the scope of formula calculation.
### See Also

* module [aspose.cells](../)
