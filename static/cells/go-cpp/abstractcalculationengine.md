##AbstractCalculationEngine Class
'AbstractCalculationEngine class. Encapsulates the object that represents abstractcalculationengine in Go.'
## AbstractCalculationEngine class
Represents user's custom calculation engine to extend the default calculation engine of Aspose.Cells.
```go
type AbstractCalculationEngine struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[IsParamLiteralRequired](./isparamliteralrequired/) | Indicates whether this engine needs the literal text of parameter while doing calculation. Default value is false. |
|[IsParamArrayModeRequired](./isparamarraymoderequired/) | Indicates whether this engine needs the parameter to be calculated in array mode. Default value is false.If CalculationData.GetParamValueInArrayMode(int, int, int) is required when calculating customfunctions and user has not updated the definition for them(by Workbook.UpdateCustomFunctionDefinition(CustomFunctionDefinition)),this property needs to be set as true. |
|[GetProcessBuiltInFunctions](./getprocessbuiltinfunctions/) | Whether built-in functions that have been supported by the built-in engineshould be checked and processed by this implementation.Default is false. |
|[ForceRecalculate](./forcerecalculate/) | Whether force given function to be recalculated always when calculating shared formulas. |
