##Class GridAbstractCalculationEngine
Aspose.Cells.GridWeb.Data.GridAbstractCalculationEngine class. Represents users custom calculation engine to extend the default calculation engine of Aspose.Cells
## GridAbstractCalculationEngine class
Represents user's custom calculation engine to extend the default calculation engine of Aspose.Cells.
```csharp
public abstract class GridAbstractCalculationEngine
```
## Methods
| Name | Description |
| --- | --- |
| abstract [Calculate](../../aspose.cells.gridweb.data/gridabstractcalculationengine/calculate/)(GridCalculationData) | Calculates one function with given data. |
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
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)
