##AbstractCalculationEngine.ProcessBuiltInFunctions
AbstractCalculationEngine property. Whether builtin functions that have been supported by the builtin engine should be checked and processed by this implementation. Default is false
## AbstractCalculationEngine.ProcessBuiltInFunctions property
Whether built-in functions that have been supported by the built-in engine should be checked and processed by this implementation. Default is false.
```csharp
public virtual bool ProcessBuiltInFunctions { get; }
```
### Remarks
If user needs to change the calculation logic of some built-in functions, this property should be set as true. Otherwise please leave this property as false for performance consideration.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class AbstractCalculationEnginePropertyProcessBuiltInFunctionsDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate test data
worksheet.Cells["A1"].PutValue(1);
worksheet.Cells["A2"].PutValue(2);
worksheet.Cells["A3"].PutValue(3);
worksheet.Cells["A4"].Formula = "=SUM(A1:A3)";
// Create custom calculation engines with different ProcessBuiltInFunctions values
CustomEngine engineProcessEnabled = new CustomEngine(true);
CustomEngine engineProcessDisabled = new CustomEngine(false);
// Show property values
Console.WriteLine("Engine1 ProcessBuiltInFunctions: " + engineProcessEnabled.ProcessBuiltInFunctions);
Console.WriteLine("Engine2 ProcessBuiltInFunctions: " + engineProcessDisabled.ProcessBuiltInFunctions);
// Calculate with custom engine (ProcessBuiltInFunctions = true)
CalculationOptions optionsEnabled = new CalculationOptions { CustomEngine = engineProcessEnabled };
workbook.CalculateFormula(optionsEnabled);
Console.WriteLine("Result with ProcessBuiltInFunctions=true: " + worksheet.Cells["A4"].Value);
// Calculate with custom engine (ProcessBuiltInFunctions = false)
CalculationOptions optionsDisabled = new CalculationOptions { CustomEngine = engineProcessDisabled };
workbook.CalculateFormula(optionsDisabled);
Console.WriteLine("Result with ProcessBuiltInFunctions=false: " + worksheet.Cells["A4"].Value);
workbook.Save("ProcessBuiltInFunctionsDemo.xlsx");
}
}
public class CustomEngine : AbstractCalculationEngine
{
private readonly bool _processBuiltIn;
public CustomEngine(bool processBuiltIn)
{
_processBuiltIn = processBuiltIn;
}
public override bool ProcessBuiltInFunctions => _processBuiltIn;
public override void Calculate(CalculationData data)
{
if (data.FunctionName.Equals("SUM", StringComparison.OrdinalIgnoreCase) && ProcessBuiltInFunctions)
{
double sum = 0;
for (int i = 0; i < data.ParamCount; i++)
{
object param = data.GetParamValue(i);
Aspose.Cells.ReferredArea paramArea1 = (Aspose.Cells.ReferredArea)data.GetParamValue(0);
for (int r = paramArea1.StartRow; r <= paramArea1.EndRow; r++)
{
for (int c = paramArea1.StartColumn; c <= paramArea1.EndColumn; c++)
{
object cellValue = paramArea1.GetValue(r, c);
sum += Convert.ToDouble(cellValue);
}
}
}
data.CalculatedValue = sum * 2; // Custom SUM implementation doubles the result
}
// Other functions are handled by default engine
}
public override bool ForceRecalculate(string functionName) => false;
}
}
```
### See Also
* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
