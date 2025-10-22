##AboveAverage.IsAboveAverage
AboveAverage property. Get or set the flag indicating whether the rule is an above average rule. true indicates above average. Default value is true
## AboveAverage.IsAboveAverage property
Get or set the flag indicating whether the rule is an "above average" rule. 'true' indicates 'above average'. Default value is true.
```csharp
public bool IsAboveAverage { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class AboveAveragePropertyIsAboveAverageDemo
{
public static void Run()
{
// Create a new Workbook
Workbook workbook = new Workbook();
// Get the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to demonstrate the conditional formatting
for (int i = 0; i <= 10; i++)
{
worksheet.Cells[i, 0].PutValue(i * 10);
}
// Add a conditional formatting
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
// Set the conditional format range
CellArea ca = new CellArea
{
StartRow = 0,
EndRow = 10,
StartColumn = 0,
EndColumn = 0
};
fcs.AddArea(ca);
// Add an AboveAverage condition
int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
FormatCondition fc = fcs[conditionIndex];
fc.Style.BackgroundColor = Color.Yellow;
// Configure the AboveAverage properties
fc.AboveAverage.IsAboveAverage = true;  // Highlight values above average
fc.AboveAverage.IsEqualAverage = false; // Exclude values equal to average
// Save the Excel file
workbook.Save("AboveAverageConditionDemo.xlsx");
}
}
}
```
### See Also
* class [AboveAverage](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
