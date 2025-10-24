##ColorScale.MaxColor
ColorScale property. Get or set the gradient color for the maximum value in the range
## ColorScale.MaxColor property
Get or set the gradient color for the maximum value in the range.
```csharp
public Color MaxColor { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ColorScalePropertyMaxColorDemo
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
worksheet.Cells["A5"].PutValue(50);
// Add conditional formatting
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
// Create CellArea object instead of using string
CellArea area = new CellArea();
area.StartRow = 0;
area.EndRow = 4;
area.StartColumn = 0;
area.EndColumn = 0;
fcs.AddArea(area);
// Add color scale condition
int conditionIndex = fcs.AddCondition(FormatConditionType.ColorScale);
FormatCondition fc = fcs[conditionIndex];
ColorScale colorScale = fc.ColorScale;
// Configure color scale
colorScale.Is3ColorScale = false; // Use 2-color scale for simplicity
colorScale.MinColor = Color.Green;
colorScale.MaxColor = Color.Red; // Demonstrating MaxColor property
// Set value objects
colorScale.MinCfvo.Type = FormatConditionValueType.Min;
colorScale.MaxCfvo.Type = FormatConditionValueType.Max;
// Save the workbook
workbook.Save("ColorScaleMaxColorDemo.xlsx");
}
}
}
```
### See Also
* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
