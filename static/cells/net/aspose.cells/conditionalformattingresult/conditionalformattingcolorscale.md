##ConditionalFormattingResult.ConditionalFormattingColorScale
ConditionalFormattingResult property. Gets the ColorScale object
## ConditionalFormattingResult.ConditionalFormattingColorScale property
Gets the ColorScale object.
```csharp
public ColorScale ConditionalFormattingColorScale { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class ConditionalFormattingResultPropertyConditionalFormattingColorScaleDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
CellArea ca = new CellArea { StartRow = 0, EndRow = 5, StartColumn = 0, EndColumn = 5 };
fcs.AddArea(ca);
int conditionIndex = fcs.AddCondition(FormatConditionType.ColorScale);
FormatCondition fc = fcs[conditionIndex];
fc.ColorScale.Is3ColorScale = true;
fc.ColorScale.MinColor = Color.Red;
fc.ColorScale.MidColor = Color.Yellow;
fc.ColorScale.MaxColor = Color.Green;
for (int i = 0; i <= 5; i++)
{
for (int j = 0; j <= 5; j++)
{
worksheet.Cells[i, j].PutValue(i * j);
}
}
Cell cell = worksheet.Cells["B2"];
ConditionalFormattingResult cfr = cell.GetConditionalFormattingResult();
ColorScale colorScale = cfr.ConditionalFormattingColorScale;
Console.WriteLine("ColorScale MinColor: " + colorScale.MinColor);
Console.WriteLine("ColorScale MidColor: " + colorScale.MidColor);
Console.WriteLine("ColorScale MaxColor: " + colorScale.MaxColor);
Console.WriteLine("ColorScale Result: " + cfr.ColorScaleResult);
workbook.Save("ConditionalFormattingColorScaleDemo.xlsx");
}
}
}
```
### See Also
* class [ColorScale](../../colorscale/)
* class [ConditionalFormattingResult](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
