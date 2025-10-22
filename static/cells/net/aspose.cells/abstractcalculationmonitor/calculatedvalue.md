##AbstractCalculationMonitor.CalculatedValue
AbstractCalculationMonitor property. Gets the newly calculated value of the cell. Should be used only in AfterCalculate
## AbstractCalculationMonitor.CalculatedValue property
Gets the newly calculated value of the cell. Should be used only in [`AfterCalculate`](../aftercalculate/).
```csharp
public object CalculatedValue { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CustomCalculationMonitor : AbstractCalculationMonitor
{
public override void AfterCalculate(int sheetIndex, int rowIndex, int columnIndex)
{
if (ValueChanged)
{
Console.WriteLine($"Value changed from [{OriginalValue}] to [{CalculatedValue}]");
}
}
}
public class AbstractCalculationMonitorPropertyCalculatedValueDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Setup calculation chain
worksheet.Cells["A1"].Formula = "=1+2";
worksheet.Cells["A2"].Formula = "=A1*3";
// Create and attach monitor
CustomCalculationMonitor monitor = new CustomCalculationMonitor();
CalculationOptions options = new CalculationOptions();
options.CalculationMonitor = monitor;
// Trigger calculation which will invoke our monitor
workbook.CalculateFormula(options);
// Change a value to trigger value change notification
worksheet.Cells["A1"].Value = 5;
workbook.CalculateFormula(options);
}
}
}
```
### See Also
* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
