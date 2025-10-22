##ConditionalFormattingResult.ConditionalFormattingDataBar
ConditionalFormattingResult property. Gets the DataBar object
## ConditionalFormattingResult.ConditionalFormattingDataBar property
Gets the DataBar object.
```csharp
public DataBar ConditionalFormattingDataBar { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ConditionalFormattingResultPropertyConditionalFormattingDataBarDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample values
worksheet.Cells["A1"].PutValue(-6);
worksheet.Cells["A2"].PutValue(-4);
worksheet.Cells["A3"].PutValue(-2);
worksheet.Cells["A4"].PutValue(0);
worksheet.Cells["A5"].PutValue(2);
worksheet.Cells["A6"].PutValue(4);
worksheet.Cells["A7"].PutValue(6);
// Add data bar conditional formatting
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
CellArea area = new CellArea();
area.StartRow = 0;
area.StartColumn = 0;
area.EndRow = 6;
area.EndColumn = 0;
fcc.AddArea(area);
int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
FormatCondition condition = fcc[conditionIndex];
condition.DataBar.MinCfvo.Type = FormatConditionValueType.Min;
condition.DataBar.MaxCfvo.Type = FormatConditionValueType.Max;
condition.DataBar.Color = System.Drawing.Color.Green;
// Calculate formulas and apply formatting
workbook.CalculateFormula();
// Get conditional formatting result and demonstrate DataBar properties
Cell cell = worksheet.Cells["A1"];
ConditionalFormattingResult formattingResult = cell.GetConditionalFormattingResult();
Console.WriteLine("DataBar Min Value: " + formattingResult.ConditionalFormattingDataBar.MinCfvo.Value);
Console.WriteLine("DataBar Max Value: " + formattingResult.ConditionalFormattingDataBar.MaxCfvo.Value);
Console.WriteLine("DataBar Color: " + formattingResult.ConditionalFormattingDataBar.Color);
}
}
}
```
### See Also
* class [DataBar](../../databar/)
* class [ConditionalFormattingResult](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
