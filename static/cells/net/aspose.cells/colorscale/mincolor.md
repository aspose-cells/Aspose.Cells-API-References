##ColorScale.MinColor
ColorScale property. Get or set the gradient color for the minimum value in the range
## ColorScale.MinColor property
Get or set the gradient color for the minimum value in the range.
```csharp
public Color MinColor { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ColorScalePropertyMinColorDemo
{
public static void Run()
{
// Create a new workbook and get the first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue(30);
worksheet.Cells["A4"].PutValue(40);
// Add conditional formatting
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
// Create CellArea object instead of using string
CellArea area = new CellArea();
area.StartRow = 0;
area.StartColumn = 0;
area.EndRow = 3;
area.EndColumn = 0;
fcs.AddArea(area);
int conditionIndex = fcs.AddCondition(FormatConditionType.ColorScale);
FormatCondition fc = fcs[conditionIndex];
// Configure color scale
ColorScale colorScale = fc.ColorScale;
colorScale.MinColor = Color.Green;
colorScale.MidColor = Color.Yellow;
colorScale.MaxColor = Color.Red;
// Set value types
colorScale.MinCfvo.Type = FormatConditionValueType.Min;
colorScale.MidCfvo.Type = FormatConditionValueType.Percentile;
colorScale.MidCfvo.Value = 50;
colorScale.MaxCfvo.Type = FormatConditionValueType.Max;
// Save the workbook
workbook.Save("ColorScaleMinColorDemo.xlsx");
}
}
}
```
### See Also
* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
