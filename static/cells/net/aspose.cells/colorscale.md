##Class ColorScale
Aspose.Cells.ColorScale class. Describe the ColorScale conditional formatting rule. This conditional formatting rule creates a gradated color scale on the cells
## ColorScale class
Describe the ColorScale conditional formatting rule. This conditional formatting rule creates a gradated color scale on the cells.
```csharp
public class ColorScale
```
## Properties
| Name | Description |
| --- | --- |
| [Is3ColorScale](../../aspose.cells/colorscale/is3colorscale/) { get; set; } | Indicates whether conditional formatting is 3 color scale. |
| [MaxCfvo](../../aspose.cells/colorscale/maxcfvo/) { get; } | Get or set this ColorScale's max value object. Cannot set null or CFValueObject with type FormatConditionValueType.Min to it. |
| [MaxColor](../../aspose.cells/colorscale/maxcolor/) { get; set; } | Get or set the gradient color for the maximum value in the range. |
| [MidCfvo](../../aspose.cells/colorscale/midcfvo/) { get; } | Get or set this ColorScale's mid value object. Cannot set CFValueObject with type FormatConditionValueType.Max or FormatConditionValueType.Min to it. |
| [MidColor](../../aspose.cells/colorscale/midcolor/) { get; set; } | Get or set the gradient color for the middle value in the range. |
| [MinCfvo](../../aspose.cells/colorscale/mincfvo/) { get; } | Get or set this ColorScale's min value object. Cannot set null or CFValueObject with type FormatConditionValueType.Max to it. |
| [MinColor](../../aspose.cells/colorscale/mincolor/) { get; set; } | Get or set the gradient color for the minimum value in the range. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Drawing;
public class ColorScaleDemo
{
public static void ColorScaleExample()
{
// Create a new workbook and get the first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data to the worksheet
for (int i = 0; i < 10; i++)
{
for (int j = 0; j < 10; j++)
{
worksheet.Cells[i, j].PutValue(i * j);
}
}
// Add a conditional formatting rule
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
CellArea ca = new CellArea { StartRow = 0, EndRow = 9, StartColumn = 0, EndColumn = 9 };
fcs.AddArea(ca);
int conditionIndex = fcs.AddCondition(FormatConditionType.ColorScale);
FormatCondition fc = fcs[conditionIndex];
// Access the ColorScale object
ColorScale colorScale = fc.ColorScale;
// Set properties for the ColorScale
colorScale.Is3ColorScale = true;
colorScale.MinColor = Color.Green;
colorScale.MidColor = Color.Yellow;
colorScale.MaxColor = Color.Red;
// Set the min, mid, and max value objects
ConditionalFormattingValue minCfvo = colorScale.MinCfvo;
minCfvo.Type = FormatConditionValueType.Min;
minCfvo.Value = null;
ConditionalFormattingValue midCfvo = colorScale.MidCfvo;
midCfvo.Type = FormatConditionValueType.Percentile;
midCfvo.Value = 50;
ConditionalFormattingValue maxCfvo = colorScale.MaxCfvo;
maxCfvo.Type = FormatConditionValueType.Max;
maxCfvo.Value = null;
// Save the workbook
workbook.Save("ColorScaleExample.xlsx");
workbook.Save("ColorScaleExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
