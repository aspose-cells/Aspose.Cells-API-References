##Cell.GetConditionalFormattingResult
Cell method. Get the result of the conditional formatting
## Cell.GetConditionalFormattingResult method
Get the result of the conditional formatting.
```csharp
public ConditionalFormattingResult GetConditionalFormattingResult()
```
### Remarks
Returns null if no conditional formatting is applied to this cell,
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellMethodGetConditionalFormattingResultDemo
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
// Add conditional formatting
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
CellArea area = new CellArea();
area.StartRow = 0;
area.StartColumn = 0;
area.EndRow = 3;
area.EndColumn = 0;
fcc.AddArea(area);
// Set condition and style
int conditionIndex = fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "15", "35");
Style style = workbook.CreateStyle();
style.Font.Color = System.Drawing.Color.Red;
fcc[conditionIndex].Style = style;
// Get conditional formatting result for a cell
Cell cell = worksheet.Cells["A2"];
ConditionalFormattingResult result = cell.GetConditionalFormattingResult();
// Output result
Console.WriteLine("Cell A2 meets condition: " + (result.ConditionalStyle != null));
Console.WriteLine("Applied font color: " + result.ConditionalStyle.Font.Color);
}
}
}
```
### See Also
* class [ConditionalFormattingResult](../../conditionalformattingresult/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
