##GridAbstractCalculationEngine class
## GridAbstractCalculationEngine class
Represents user's custom calculation engine to extend the default calculation engine of Aspose.Cells.
The GridAbstractCalculationEngine type exposes the following members:
### Methods
| Method | Description |
| :- | :- |
| [calculate](/cells/python-net/aspose.cellsgridjs/gridabstractcalculationengine/calculate/#aspose.cellsgridjs.GridCalculationData) | Calculates one function with given data. |
### Remarks
User should not modify any part of the Workbook directly in this implementation(except the calculated result of the custom function, which can be set by GridCalculationData.CalculatedValue property).
Otherwise unexpected result or Exception may be caused.
If user needs to change other data than calculated result in the implementation for some custom functions,
For example, change cell's formula, style, ...etc., user should gather those data in this implementation and change them out of the scope of formula calculation.
### See Also
* module [`aspose.cellsgridjs`](..)
