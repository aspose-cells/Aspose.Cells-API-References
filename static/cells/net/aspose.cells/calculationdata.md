##Class CalculationData
Aspose.Cells.CalculationData class. Represents the required data when calculating one function such as function name parameters ...etc
## CalculationData class
Represents the required data when calculating one function, such as function name, parameters, ...etc.
```csharp
public class CalculationData
```
## Properties
| Name | Description |
| --- | --- |
| [CalculatedValue](../../aspose.cells/calculationdata/calculatedvalue/) { get; set; } | Gets or sets the calculated value for this function. |
| [Cell](../../aspose.cells/calculationdata/cell/) { get; } | Gets the Cell object where the function is in. |
| [CellColumn](../../aspose.cells/calculationdata/cellcolumn/) { get; } | Gets the column index of the cell where the function is in. |
| [CellRow](../../aspose.cells/calculationdata/cellrow/) { get; } | Gets the row index of the cell where the function is in. |
| [FunctionName](../../aspose.cells/calculationdata/functionname/) { get; } | Gets the function name to be calculated. |
| [ParamCount](../../aspose.cells/calculationdata/paramcount/) { get; } | Gets the count of parameters |
| [Workbook](../../aspose.cells/calculationdata/workbook/) { get; } | Gets the Workbook object where the function is in. |
| [Worksheet](../../aspose.cells/calculationdata/worksheet/) { get; } | Gets the Worksheet object where the function is in. |
## Methods
| Name | Description |
| --- | --- |
| [GetParamText](../../aspose.cells/calculationdata/getparamtext/)(int) | Gets the literal text of the parameter at given index. |
| [GetParamValue](../../aspose.cells/calculationdata/getparamvalue/)(int) | Gets the represented value object of the parameter at given index. |
| [GetParamValueInArrayMode](../../aspose.cells/calculationdata/getparamvalueinarraymode/)(int, int, int) | Gets the value(s) of the parameter at given index. If the parameter is some kind of expression that needs to be calculated, then it will be calculated in array mode. |
### Remarks
All objects provided by this class are for "read" purpose only. User should not change any data in the Workbook during the formula calculation process, Otherwise unexpected result or Exception may be caused.
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
