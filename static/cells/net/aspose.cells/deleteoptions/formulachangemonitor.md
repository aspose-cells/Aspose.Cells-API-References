##DeleteOptions.FormulaChangeMonitor
DeleteOptions property. Gets/sets the monitor for tracking changes caused by the deletion
## DeleteOptions.FormulaChangeMonitor property
Gets/sets the monitor for tracking changes caused by the deletion.
```csharp
public AbstractFormulaChangeMonitor FormulaChangeMonitor { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DeleteOptionsPropertyFormulaChangeMonitorDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
Cells cells = sheet.Cells;
// Set up test data
cells["A1"].Formula = "=A5";
cells["A5"].Value = 10;
// Add conditional formatting
int index = sheet.ConditionalFormattings.Add();
FormatConditionCollection fcc = sheet.ConditionalFormattings[index];
fcc.Add(CellArea.CreateCellArea(0, 3, 1, 4), FormatConditionType.Expression,
OperatorType.Equal, "=A8>0", "");
// Create and assign monitor
CustomFormulaChangeMonitor monitor = new CustomFormulaChangeMonitor();
DeleteOptions options = new DeleteOptions
{
FormulaChangeMonitor = monitor,
UpdateReference = true
};
// Delete row which should trigger formula changes
cells.DeleteRows(2, 1, options);
// Output monitoring results
Console.WriteLine("Cell formula changes detected: " + monitor.CellChangesDetected);
Console.WriteLine("Format condition changes detected: " + monitor.FormatConditionChangesDetected);
}
}
public class CustomFormulaChangeMonitor : AbstractFormulaChangeMonitor
{
public bool CellChangesDetected { get; private set; }
public bool FormatConditionChangesDetected { get; private set; }
public override void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
{
CellChangesDetected = true;
Console.WriteLine($"Cell formula changed at Sheet {sheetIndex}, Row {rowIndex}, Column {columnIndex}");
}
public override void OnFormatConditionFormulaChanged(FormatCondition fc)
{
FormatConditionChangesDetected = true;
Console.WriteLine("Format condition formula changed");
}
}
}
```
### See Also
* class [AbstractFormulaChangeMonitor](../../abstractformulachangemonitor/)
* class [DeleteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
