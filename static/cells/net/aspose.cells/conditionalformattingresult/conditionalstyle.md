##ConditionalFormattingResult.ConditionalStyle
ConditionalFormattingResult property. Gets the conditional result style
## ConditionalFormattingResult.ConditionalStyle property
Gets the conditional result style.
```csharp
public Style ConditionalStyle { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class ConditionalFormattingResultPropertyConditionalStyleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Value");
worksheet.Cells["A2"].PutValue(10);
worksheet.Cells["A3"].PutValue(20);
worksheet.Cells["A4"].PutValue(30);
// Add conditional formatting
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
fcc.AddArea(new CellArea { StartRow = 1, StartColumn = 0, EndRow = 3, EndColumn = 0 });
// Create condition and set style
int conditionIndex = fcc.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "15", null);
FormatCondition fc = fcc[conditionIndex];
Style style = workbook.CreateStyle();
style.Font.Color = Color.Red;
fc.Style = style;
// Get cell with conditional formatting
Cell cell = worksheet.Cells["A3"];
Style conditionalStyle = cell.GetConditionalFormattingResult().ConditionalStyle;
// Output the color to demonstrate the property
Console.WriteLine("Conditional Style Font Color: " + conditionalStyle.Font.Color);
}
}
}
```
### See Also
* class [Style](../../style/)
* class [ConditionalFormattingResult](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
