##DataBar.MaxCfvo
DataBar property. Get or set this DataBars max value object. Cannot set null or CFValueObject with type FormatConditionValueType.Min to it
## DataBar.MaxCfvo property
Get or set this DataBar's max value object. Cannot set null or CFValueObject with type FormatConditionValueType.Min to it.
```csharp
public ConditionalFormattingValue MaxCfvo { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DataBarPropertyMaxCfvoDemo
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
worksheet.Cells["A4"].PutValue(40);
// Add data bar conditional formatting
int idx = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcc = worksheet.ConditionalFormattings[idx];
CellArea area = new CellArea();
area.StartRow = 0;
area.EndRow = 3;
area.StartColumn = 0;
area.EndColumn = 0;
fcc.AddArea(area);
// Add data bar
int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
DataBar dataBar = fcc[conditionIndex].DataBar;
// Set MaxCfvo value
dataBar.MaxCfvo.Type = FormatConditionValueType.Max;
dataBar.MaxCfvo.Value = 50;
// Save the workbook
workbook.Save("DataBarMaxCfvoDemo.xlsx");
}
}
}
```
### See Also
* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
