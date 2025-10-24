##FormatCondition.ColorScale
FormatCondition property. Get the conditional formattings ColorScale instance. The default instance is a greenyellowred 3ColorScale . Valid only for type  ColorScale
## FormatCondition.ColorScale property
Get the conditional formatting's "ColorScale" instance. The default instance is a "green-yellow-red" 3ColorScale . Valid only for type = ColorScale.
```csharp
public ColorScale ColorScale { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class FormatConditionPropertyColorScaleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
for (int i = 0; i < 10; i++)
{
worksheet.Cells[i, 0].PutValue(i + 1);
}
// Add a color scale conditional formatting
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
// Set the range for the conditional formatting
CellArea area = new CellArea();
area.StartRow = 0;
area.EndRow = 9;
area.StartColumn = 0;
area.EndColumn = 0;
fcs.AddArea(area);
// Set the color scale properties
fcs.AddCondition(FormatConditionType.ColorScale);
FormatCondition fc = fcs[0];
fc.ColorScale.MinCfvo.Type = FormatConditionValueType.Min;
fc.ColorScale.MinColor = Color.Red;
fc.ColorScale.MidCfvo.Type = FormatConditionValueType.Percentile;
fc.ColorScale.MidCfvo.Value = 50;
fc.ColorScale.MidColor = Color.Yellow;
fc.ColorScale.MaxCfvo.Type = FormatConditionValueType.Max;
fc.ColorScale.MaxColor = Color.Green;
// Save the workbook
workbook.Save("ColorScaleExample.xlsx");
}
}
}
```
### See Also
* class [ColorScale](../../colorscale/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
