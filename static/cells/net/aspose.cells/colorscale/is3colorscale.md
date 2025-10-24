##ColorScale.Is3ColorScale
ColorScale property. Indicates whether conditional formatting is 3 color scale
## ColorScale.Is3ColorScale property
Indicates whether conditional formatting is 3 color scale.
```csharp
public bool Is3ColorScale { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class ColorScalePropertyIs3ColorScaleDemo
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
fc.ColorScale.MinCfvo.Type = FormatConditionValueType.Min;
fc.ColorScale.MinColor = Color.Blue;
fc.ColorScale.MidCfvo.Type = FormatConditionValueType.Percentile;
fc.ColorScale.MidCfvo.Value = 50;
fc.ColorScale.MidColor = Color.Yellow;
fc.ColorScale.MaxCfvo.Type = FormatConditionValueType.Max;
fc.ColorScale.MaxColor = Color.Red;
workbook.Save("ColorScale3ColorExample.xlsx");
}
}
}
```
### See Also
* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
