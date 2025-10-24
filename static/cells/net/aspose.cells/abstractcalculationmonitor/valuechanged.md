##AbstractCalculationMonitor.ValueChanged
AbstractCalculationMonitor property. Whether the cells value has been changed after the calculation. Should be used only in AfterCalculate
## AbstractCalculationMonitor.ValueChanged property
Whether the cell's value has been changed after the calculation. Should be used only in [`AfterCalculate`](../aftercalculate/).
```csharp
public bool ValueChanged { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CustomCalculationMonitor2 : AbstractCalculationMonitor
{
public bool Changed { get; set; }
public override void AfterCalculate(int sheetIndex, int rowIndex, int colIndex)
{
if (ValueChanged)
{
Changed = true;
Console.WriteLine($"Value changed from [{OriginalValue}] to [{CalculatedValue}]");
}
}
}
public class AbstractCalculationMonitorPropertyValueChangedDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set initial value
worksheet.Cells["A1"].Value = 10;
worksheet.Cells["A2"].Formula = "=A1*2";
// Create and set calculation monitor
CustomCalculationMonitor2 monitor = new CustomCalculationMonitor2();
CalculationOptions options = new CalculationOptions();
options.CalculationMonitor = monitor;
// First calculation
workbook.CalculateFormula(options);
Console.WriteLine($"First calculation - Changed: {monitor.Changed}");
// Change value and recalculate
worksheet.Cells["A1"].Value = 20;
monitor.Changed = false;
workbook.CalculateFormula(options);
Console.WriteLine($"Second calculation - Changed: {monitor.Changed}");
}
}
}
```
### See Also
* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
