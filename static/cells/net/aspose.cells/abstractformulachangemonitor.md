##Class AbstractFormulaChangeMonitor
Aspose.Cells.AbstractFormulaChangeMonitor class. Monitor for user to track the change of formulas during certain operations
## AbstractFormulaChangeMonitor class
Monitor for user to track the change of formulas during certain operations.
```csharp
public abstract class AbstractFormulaChangeMonitor
```
## Methods
| Name | Description |
| --- | --- |
| virtual [OnCellFormulaChanged](../../aspose.cells/abstractformulachangemonitor/oncellformulachanged/)(int, int, int) | The event that will be triggered when the formula in a cell is changed. |
| virtual [OnFormatConditionFormulaChanged](../../aspose.cells/abstractformulachangemonitor/onformatconditionformulachanged/)(FormatCondition) | The event that will be triggered when the formula of FormatCondition is changed. |
### Remarks
For example, while deleting/inserting range of cells, formulas of other cells may be changed because of the shift of references. Please note, methods in the monitor may be invoked multiple times for one object which contains the formula.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsClassAbstractFormulaChangeMonitorDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet worksheet = wb.Worksheets[0];
// Set some formulas in cells
worksheet.Cells["A1"].Formula = "=B1+C1";
worksheet.Cells["B1"].Formula = "=D1*2";
worksheet.Cells["C1"].Value = 5;
worksheet.Cells["D1"].Value = 10;
InsertOptions options = new InsertOptions();
options.FormulaChangeMonitor = new MyFormulaChangeMonitor(wb.Worksheets);
// Insert rows which will trigger formula changes
worksheet.Cells.InsertRows(0, 2, options);
}
}
public class MyFormulaChangeMonitor : AbstractFormulaChangeMonitor
{
private readonly WorksheetCollection mWorksheets;
public MyFormulaChangeMonitor(WorksheetCollection worksheets)
{
mWorksheets = worksheets;
}
public override void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
{
Console.WriteLine($"Formula changed in {mWorksheets[sheetIndex].Name}!{CellsHelper.CellIndexToName(rowIndex, columnIndex)}");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
