##DataBar.AxisColor
DataBar property. Gets the color of the axis for cells with conditional formatting as data bars
## DataBar.AxisColor property
Gets the color of the axis for cells with conditional formatting as data bars.
```csharp
public Color AxisColor { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DataBarPropertyAxisColorDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Set sample data
sheet.Cells["E3"].PutValue(10);
sheet.Cells["E4"].PutValue(20);
sheet.Cells["F3"].PutValue(30);
sheet.Cells["F4"].PutValue(40);
sheet.Cells["G3"].PutValue(-15);
sheet.Cells["G4"].PutValue(-25);
// Add data bar conditional formatting
int formatIndex = sheet.ConditionalFormattings.Add();
FormatConditionCollection conds = sheet.ConditionalFormattings[formatIndex];
int idx = conds.AddCondition(FormatConditionType.DataBar);
FormatCondition cond = conds[idx];
// Set data bar properties
cond.DataBar.Color = Color.Orange;
cond.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
cond.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
cond.DataBar.ShowValue = false;
cond.DataBar.BarBorder.Type = DataBarBorderType.Solid;
cond.DataBar.BarBorder.Color = Color.Plum;
cond.DataBar.BarFillType = DataBarFillType.Solid;
// Demonstrate AxisColor property
cond.DataBar.AxisColor = Color.Red;
cond.DataBar.AxisPosition = DataBarAxisPosition.Midpoint;
// Set negative bar formatting
cond.DataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
cond.DataBar.NegativeBarFormat.Color = Color.White;
cond.DataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
cond.DataBar.NegativeBarFormat.BorderColor = Color.Yellow;
// Save the workbook
workbook.Save("DataBarAxisColorDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
