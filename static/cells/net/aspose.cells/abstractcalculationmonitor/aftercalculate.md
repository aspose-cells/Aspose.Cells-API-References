##AbstractCalculationMonitor.AfterCalculate
AbstractCalculationMonitor method. Implement this method to do business after one cell has been calculated
## AbstractCalculationMonitor.AfterCalculate method
Implement this method to do business after one cell has been calculated.
```csharp
public virtual void AfterCalculate(int sheetIndex, int rowIndex, int colIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | Int32 | Index of the sheet that the cell belongs to. |
| rowIndex | Int32 | Row index of the cell |
| colIndex | Int32 | Column index of the cell |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class AbstractCalculationMonitorMethodAfterCalculateWithInt32Int32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Setup sample formulas
worksheet.Cells["A1"].Formula = "=1+2";
worksheet.Cells["A2"].Formula = "=A1*3";
worksheet.Cells["B1"].Formula = "=NOW()"; // Volatile function
CalculationOptions options = new CalculationOptions();
var monitor = new CalculationMonitor();
options.CalculationMonitor = monitor;
try
{
workbook.CalculateFormula(options);
Console.WriteLine("Calculation completed. Check cell values and console output.");
}
catch (Exception ex)
{
Console.WriteLine($"Calculation error: {ex.Message}");
}
workbook.Save("AfterCalculateDemo.xlsx");
}
private class CalculationMonitor : AbstractCalculationMonitor
{
public override void AfterCalculate(int sheetIndex, int rowIndex, int colIndex)
{
Console.WriteLine($"Calculated cell (Sheet {sheetIndex}): Row {rowIndex}, Column {colIndex}");
Console.WriteLine($"Value changed: {ValueChanged}, Original: {OriginalValue}, New: {CalculatedValue}");
Console.WriteLine("----------------------------------");
}
}
}
}
```
### See Also
* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
