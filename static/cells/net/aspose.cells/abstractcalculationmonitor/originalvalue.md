##AbstractCalculationMonitor.OriginalValue
AbstractCalculationMonitor property. Gets the old value of the calculated cell. Should be used only in BeforeCalculate and AfterCalculate
## AbstractCalculationMonitor.OriginalValue property
Gets the old value of the calculated cell. Should be used only in [`BeforeCalculate`](../beforecalculate/) and [`AfterCalculate`](../aftercalculate/).
```csharp
public object OriginalValue { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CustomCalculationMonitor1 : AbstractCalculationMonitor
{
public override void AfterCalculate(int sheetIndex, int rowIndex, int colIndex)
{
if (ValueChanged)
{
Console.WriteLine($"Value changed from [{OriginalValue}] to [{CalculatedValue}]");
}
}
}
public class AbstractCalculationMonitorPropertyOriginalValueDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set initial value
worksheet.Cells["A1"].PutValue(10);
// Add formula that will change the value
worksheet.Cells["A2"].Formula = "=A1*2";
// Set calculation monitor
CalculationOptions options = new CalculationOptions();
options.CalculationMonitor = new CustomCalculationMonitor1();
// Recalculate formulas - this will trigger the monitor
workbook.CalculateFormula(options);
// Change the original value to demonstrate the monitor
worksheet.Cells["A1"].PutValue(20);
workbook.CalculateFormula(options);
}
}
}
```
### See Also
* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
