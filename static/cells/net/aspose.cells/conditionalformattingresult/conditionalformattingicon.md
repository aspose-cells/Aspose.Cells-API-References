##ConditionalFormattingResult.ConditionalFormattingIcon
ConditionalFormattingResult property. Gets the image of icon set
## ConditionalFormattingResult.ConditionalFormattingIcon property
Gets the image of icon set.
```csharp
public ConditionalFormattingIcon ConditionalFormattingIcon { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ConditionalFormattingResultPropertyConditionalFormattingIconDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data and conditional formatting
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue(30);
// Add icon set conditional formatting
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
CellArea area = new CellArea();
area.StartRow = 0;
area.StartColumn = 0;
area.EndRow = 2;
area.EndColumn = 0;
fcc.AddArea(area);
int conditionIndex = fcc.AddCondition(FormatConditionType.IconSet);
FormatCondition condition = fcc[conditionIndex];
condition.IconSet.Type = IconSetType.TrafficLights31;
// Calculate formulas and get conditional formatting result
workbook.CalculateFormula();
ConditionalFormattingResult result = worksheet.Cells["A1"].GetConditionalFormattingResult();
// Demonstrate ConditionalFormattingIcon property
if (result != null && result.ConditionalFormattingIcon != null)
{
Console.WriteLine("Icon Type: " + result.ConditionalFormattingIcon.Type);
Console.WriteLine("Icon Index: " + result.ConditionalFormattingIcon.Index);
}
}
}
}
```
### See Also
* class [ConditionalFormattingIcon](../../conditionalformattingicon/)
* class [ConditionalFormattingResult](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
