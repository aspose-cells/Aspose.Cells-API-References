##CalculationOptions.CustomEngine
CalculationOptions property. The custom formula calculation engine to extend the default calculation engine of Aspose.Cells
## CalculationOptions.CustomEngine property
The custom formula calculation engine to extend the default calculation engine of Aspose.Cells.
```csharp
public AbstractCalculationEngine CustomEngine { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CalculationOptionsPropertyCustomEngineDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
// Set HYPERLINK formula in cell A1
sheet.Cells["A1"].Formula = "=HYPERLINK(\"http://example.com\",\"Click Here\")";
// Create custom engine that processes HYPERLINK function
CustomEngineForHyperlink customEngine = new CustomEngineForHyperlink(true);
// Set calculation options with custom engine
CalculationOptions options = new CalculationOptions();
options.CustomEngine = customEngine;
// Calculate formulas with custom engine
wb.CalculateFormula(options);
Console.WriteLine("Custom engine invoked: " + customEngine.Invoked);
}
}
public class CustomEngineForHyperlink : AbstractCalculationEngine
{
public bool Invoked { get; private set; }
private readonly bool _shouldProcess;
public CustomEngineForHyperlink(bool shouldProcess)
{
_shouldProcess = shouldProcess;
}
public override void Calculate(CalculationData data)
{
if (data.FunctionName == "HYPERLINK" && _shouldProcess)
{
Invoked = true;
data.CalculatedValue = "[Custom Processed] " + data.GetParamText(1);
}
// Don't call base.Calculate() as it's abstract
// Just let the default calculation happen for other functions
}
}
}
```
### See Also
* class [AbstractCalculationEngine](../../abstractcalculationengine/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
