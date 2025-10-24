##AbstractCalculationMonitor.BeforeCalculate
AbstractCalculationMonitor method. Implement this method to do business before calculating one cell
## AbstractCalculationMonitor.BeforeCalculate method
Implement this method to do business before calculating one cell.
```csharp
public virtual void BeforeCalculate(int sheetIndex, int rowIndex, int colIndex)
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
public class CustomCalculationMonitor2 : AbstractCalculationMonitor
{
public override void BeforeCalculate(int sheetIndex, int rowIndex, int colIndex)
{
Console.WriteLine($"BeforeCalculate called for Sheet {sheetIndex}, Row {rowIndex}, Column {colIndex}");
Console.WriteLine($"Original Value: {this.OriginalValue ?? "null"}");
}
public override void AfterCalculate(int sheetIndex, int rowIndex, int colIndex)
{
Console.WriteLine($"AfterCalculate called for Sheet {sheetIndex}, Row {rowIndex}, Column {colIndex}");
Console.WriteLine($"New Value: {this.CalculatedValue ?? "null"}, Value Changed: {this.ValueChanged}");
}
}
public class AbstractCalculationMonitorMethodBeforeCalculateWithInt32Int32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Setup calculation dependencies
worksheet.Cells["B1"].PutValue(5);
worksheet.Cells["C1"].PutValue(7);
worksheet.Cells["A1"].Formula = "=B1 + C1";
CustomCalculationMonitor2 monitor = new CustomCalculationMonitor2();
CalculationOptions options = new CalculationOptions { CalculationMonitor = monitor };
try
{
Console.WriteLine("Starting spreadsheet calculation...");
workbook.CalculateFormula(options);
Console.WriteLine("\nFinal cell values:");
Console.WriteLine($"A1 calculated value: {worksheet.Cells["A1"].Value}");
Console.WriteLine($"B1 value: {worksheet.Cells["B1"].Value}");
Console.WriteLine($"C1 value: {worksheet.Cells["C1"].Value}");
}
catch (Exception ex)
{
Console.WriteLine($"Calculation error: {ex.Message}");
}
workbook.Save("BeforeCalculateDemo.xlsx");
}
}
}
```
### See Also
* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
