##AbstractFormulaChangeMonitor.OnCellFormulaChanged
AbstractFormulaChangeMonitor method. The event that will be triggered when the formula in a cell is changed
## AbstractFormulaChangeMonitor.OnCellFormulaChanged method
The event that will be triggered when the formula in a cell is changed.
```csharp
public virtual void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | Int32 | The sheet index of the changed cell |
| rowIndex | Int32 | The row index of the changed cell |
| columnIndex | Int32 | The column index of the changed cell |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class AbstractFormulaChangeMonitorMethodOnCellFormulaChangedWithInt32Int32Int32Demo : AbstractFormulaChangeMonitor
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create an instance of our demo class that inherits from AbstractFormulaChangeMonitor
var monitor = new AbstractFormulaChangeMonitorMethodOnCellFormulaChangedWithInt32Int32Int32Demo();
// Set some formula in a cell to trigger the change
worksheet.Cells["A1"].Formula = "=SUM(B1:B10)";
try
{
// Call OnCellFormulaChanged with sheet index 0, row 0, column 0 (A1)
monitor.OnCellFormulaChanged(0, 0, 0);
Console.WriteLine("OnCellFormulaChanged called successfully for cell A1");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing OnCellFormulaChanged method: {ex.Message}");
}
// Save the workbook
workbook.Save("OnCellFormulaChangedDemo.xlsx");
}
public override void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
{
// Implementation to handle formula change
Console.WriteLine($"Formula changed in sheet {sheetIndex} at row {rowIndex}, column {columnIndex}");
}
}
}
```
### See Also
* class [AbstractFormulaChangeMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
