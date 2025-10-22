##Class GridAbstractCalculationEngine
Aspose.Cells.GridJs.GridAbstractCalculationEngine class. Represents users custom calculation engine to extend the default calculation engine of Aspose.Cells
## GridAbstractCalculationEngine class
Represents user's custom calculation engine to extend the default calculation engine of Aspose.Cells.
```csharp
public abstract class GridAbstractCalculationEngine
```
## Methods
| Name | Description |
| --- | --- |
| abstract [Calculate](../../aspose.cells.gridjs/gridabstractcalculationengine/calculate/)(GridCalculationData) | Calculates one function with given data. |
### Remarks
User should not modify any part of the Workbook directly in this implementation(except the calculated result of the custom function, which can be set by GridCalculationData.CalculatedValue property). Otherwise unexpected result or Exception may be caused. If user needs to change other data than calculated result in the implementation for some custom functions, For example, change cell's formula, style, ...etc., user should gather those data in this implementation and change them out of the scope of formula calculation.
### Examples
```csharp
[C#]
class MyEngine : GridAbstractCalculationEngine
{
public override void Calculate(GridCalculationData data)
{
string funcName = data.FunctionName.ToUpper();
if ("MYFUNC".Equals(funcName))
{
//do calculation for MYFUNC here
int count = data.ParamCount;
object res = null;
for (int i = 0; i < count; i++)
{
object pv = data.GetParamValue(i);
if (pv is GridReferredArea)
{
GridReferredArea ra = (GridReferredArea)pv;
pv = ra.GetValue(0, 0);
}
//process the parameter here
//res = ...;
}
data.CalculatedValue = res;
}
}
}
```
### See Also
* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)
