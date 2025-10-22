##ConditionalFormattingValue.IsGTE
ConditionalFormattingValue property. Get or set the Greater Than Or Equal flag. Use only for icon sets determines whether this threshold value uses the greater than or equal to operator. false indicates greater than is used instead of greater than or equal to. Default value is true
## ConditionalFormattingValue.IsGTE property
Get or set the Greater Than Or Equal flag. Use only for icon sets, determines whether this threshold value uses the greater than or equal to operator. 'false' indicates 'greater than' is used instead of 'greater than or equal to'. Default value is true.
```csharp
public bool IsGTE { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class ConditionalFormattingValuePropertyIsGTEDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet ws = workbook.Worksheets[0];
// Add sample data
ws.Cells["A1"].PutValue(1);
ws.Cells["A2"].PutValue(2);
ws.Cells["A3"].PutValue(3);
ws.Cells["A4"].PutValue(4);
ws.Cells["A5"].PutValue(5);
// Add conditional formatting
int index = ws.ConditionalFormattings.Add();
FormatConditionCollection fcc = ws.ConditionalFormattings[index];
fcc.AddArea(CellArea.CreateCellArea("A1", "A5"));
// Create color scale format
index = fcc.AddCondition(FormatConditionType.ColorScale);
FormatCondition fc = fcc[index];
// Configure 2-color scale
fc.ColorScale.Is3ColorScale = false;
// Set max value format (demonstrating IsGTE)
fc.ColorScale.MaxCfvo.IsGTE = true;
fc.ColorScale.MaxCfvo.Type = FormatConditionValueType.Max;
fc.ColorScale.MaxColor = Color.Yellow;
// Set min value format
fc.ColorScale.MinCfvo.IsGTE = true;
fc.ColorScale.MinCfvo.Type = FormatConditionValueType.Min;
fc.ColorScale.MinColor = Color.Red;
// Save the workbook
workbook.Save("ConditionalFormattingValuePropertyIsGTEDemo_out.xlsx");
}
}
}
```
### See Also
* class [ConditionalFormattingValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
