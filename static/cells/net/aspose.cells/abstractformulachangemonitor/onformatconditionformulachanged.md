##AbstractFormulaChangeMonitor.OnFormatConditionFormulaChanged
AbstractFormulaChangeMonitor method. The event that will be triggered when the formula of FormatCondition is changed
## AbstractFormulaChangeMonitor.OnFormatConditionFormulaChanged method
The event that will be triggered when the formula of FormatCondition is changed.
```csharp
public virtual void OnFormatConditionFormulaChanged(FormatCondition fc)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fc | FormatCondition | The FormatCondition object whose formula is changed |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class AbstractFormulaChangeMonitorMethodOnFormatConditionFormulaChangedWithFormatConditionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue(30);
// Create a conditional formatting
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
// Create format condition
int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");
FormatCondition fc = fcs[conditionIndex];
fc.Style = workbook.CreateStyle();
fc.Style.Font.Color = System.Drawing.Color.Red;
// Create custom monitor
var monitor = new CustomFormulaChangeMonitor();
try
{
// Call the OnFormatConditionFormulaChanged method
monitor.OnFormatConditionFormulaChanged(fc);
Console.WriteLine("Method executed successfully with FormatCondition parameter");
// Apply the conditional formatting to a range
CellArea area = new CellArea();
area.StartRow = 0;
area.StartColumn = 0;
area.EndRow = 2;
area.EndColumn = 0;
fcs.AddArea(area);
}
catch (Exception ex)
{
Console.WriteLine($"Error executing OnFormatConditionFormulaChanged method: {ex.Message}");
}
workbook.Save("MethodOnFormatConditionFormulaChangedDemo.xlsx");
}
}
public class CustomFormulaChangeMonitor : AbstractFormulaChangeMonitor
{
public override void OnFormatConditionFormulaChanged(FormatCondition fc)
{
Console.WriteLine($"Format condition formula changed. Type: {fc.Type}, Formula1: {fc.Formula1}, Formula2: {fc.Formula2}");
}
}
}
```
### See Also
* class [FormatCondition](../../formatcondition/)
* class [AbstractFormulaChangeMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
