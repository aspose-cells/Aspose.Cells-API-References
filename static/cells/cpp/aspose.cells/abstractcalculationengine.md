##Aspose::Cells::AbstractCalculationEngine class
'Aspose::Cells::AbstractCalculationEngine class. Represents user''s custom calculation engine to extend the default calculation engine of Aspose.Cells in C++.'
## AbstractCalculationEngine class
Represents user's custom calculation engine to extend the default calculation engine of [Aspose.Cells](../).
```cpp
class AbstractCalculationEngine
```
## Methods
| Method | Description |
| --- | --- |
| virtual [Calculate(CalculationData\& data)](./calculate/) | Calculates one function with given data. |
| virtual [ForceRecalculate(const U16String\& functionName)](./forcerecalculate/) | Whether force given function to be recalculated always when calculating shared formulas. |
| virtual [GetProcessBuiltInFunctions()](./getprocessbuiltinfunctions/) | Whether built-in functions that have been supported by the built-in engine should be checked and processed by this implementation. Default is false. |
| virtual [IsParamArrayModeRequired()](./isparamarraymoderequired/) | Indicates whether this engine needs the parameter to be calculated in array mode. Default value is false. If CalculationData.GetParamValueInArrayMode(int, int, int) is required when calculating custom functions and user has not updated the definition for them (by Workbook.UpdateCustomFunctionDefinition(CustomFunctionDefinition)), this property needs to be set as true. |
| virtual [IsParamLiteralRequired()](./isparamliteralrequired/) | Indicates whether this engine needs the literal text of parameter while doing calculation. Default value is false. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Remarks
User should not modify any part of the [Workbook](../workbook/) directly in this implementation(except the calculated result of the custom function, which can be set by CalculationData.CalculatedValue property). Otherwise unexpected result or Exception may be caused. If user needs to change other data than calculated result in the implementation for some custom functions, for example, change cell's formula, style, ...etc., user should gather those data in this implementation and change them out of the scope of formula calculation.
## Examples
```cpp
Aspose::Cells::Startup();
class MyEngine : public AbstractCalculationEngine
{
public:
void Calculate(CalculationData& data)
{
U16String funcName = data.GetFunctionName();
if ("MYFUNC" == funcName)
{
//do calculation for MYFUNC here
int count = data.GetParamCount();
Object res;
for (int i = 0; i < count; i++)
{
Object pv = data.GetParamValue(i);
if (pv.IsReferredArea())
{
ReferredArea ra = pv.ToReferredArea();
pv = ra.GetValue(0, 0);
}
//process the parameter here
//res = ...;
}
data.SetCalculatedValue(res);
}
}
};
Workbook wb(u"custom_calc.xlsx");
MyEngine myEngine;
CalculationOptions opts;
opts.SetCustomEngine(&myEngine);
wb.CalculateFormula(opts);
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
