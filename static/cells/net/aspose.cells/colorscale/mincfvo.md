##ColorScale.MinCfvo
ColorScale property. Get or set this ColorScales min value object. Cannot set null or CFValueObject with type FormatConditionValueType.Max to it
## ColorScale.MinCfvo property
Get or set this ColorScale's min value object. Cannot set null or CFValueObject with type FormatConditionValueType.Max to it.
```csharp
public ConditionalFormattingValue MinCfvo { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ColorScalePropertyMinCfvoDemo
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
worksheet.Cells["A5"].PutValue(50);
// Create a color scale conditional formatting
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
CellArea area = new CellArea();
area.StartRow = 0;
area.EndRow = 4;
area.StartColumn = 0;
area.EndColumn = 0;
fcc.AddArea(area);
// Add color scale
int csIndex = fcc.AddCondition(FormatConditionType.ColorScale);
ColorScale cs = fcc[csIndex].ColorScale;
// Set MinCfvo properties
cs.MinCfvo.Type = FormatConditionValueType.Min;
cs.MinCfvo.Value = "0";
cs.MinColor = System.Drawing.Color.Red;
// Set MidCfvo properties
cs.MidCfvo.Type = FormatConditionValueType.Percentile;
cs.MidCfvo.Value = "50";
cs.MidColor = System.Drawing.Color.Yellow;
// Set MaxCfvo properties
cs.MaxCfvo.Type = FormatConditionValueType.Max;
cs.MaxCfvo.Value = "0";
cs.MaxColor = System.Drawing.Color.Green;
// Save the workbook
workbook.Save("ColorScaleMinCfvoDemo.xlsx");
}
}
}
```
### See Also
* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
