##CalculationOptions.CalculationMonitor
CalculationOptions property. The monitor for user to track the progress of formula calculation
## CalculationOptions.CalculationMonitor property
The monitor for user to track the progress of formula calculation.
```csharp
public AbstractCalculationMonitor CalculationMonitor { get; set; }
```
### Examples
```csharp
using System;
using System.Collections;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CalculationOptionsPropertyCalculationMonitorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set some sample formulas
worksheet.Cells["A1"].Formula = "=1+2";
worksheet.Cells["A2"].Formula = "=A1*3";
worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";
// Create calculation options with a custom monitor
CalculationOptions options = new CalculationOptions();
options.CalculationMonitor = new SampleCalculationMonitor();
// Calculate formulas with monitoring
workbook.CalculateFormula(options);
// Output results
Console.WriteLine("A1: " + worksheet.Cells["A1"].Value);
Console.WriteLine("A2: " + worksheet.Cells["A2"].Value);
Console.WriteLine("A3: " + worksheet.Cells["A3"].Value);
}
}
public class SampleCalculationMonitor : AbstractCalculationMonitor
{
public override bool OnCircular(IEnumerator circularCellsData)
{
// Handle circular references if needed
return base.OnCircular(circularCellsData);
}
public override void BeforeCalculate(int sheetIndex, int rowIndex, int columnIndex)
{
Console.WriteLine($"Before calculation: Sheet{sheetIndex}, Row{rowIndex}, Col{columnIndex}");
}
public override void AfterCalculate(int sheetIndex, int rowIndex, int columnIndex)
{
Console.WriteLine($"After calculation: Sheet{sheetIndex}, Row{rowIndex}, Col{columnIndex}");
}
}
}
```
### See Also
* class [AbstractCalculationMonitor](../../abstractcalculationmonitor/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
