##NegativeBarFormat.BorderColorType
NegativeBarFormat property. Gets whether to use the same border color as positive data bars
## NegativeBarFormat.BorderColorType property
Gets whether to use the same border color as positive data bars.
```csharp
public DataBarNegativeColorType BorderColorType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class NegativeBarFormatPropertyBorderColorTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["E3"].PutValue(-10);
sheet.Cells["E4"].PutValue(20);
sheet.Cells["F3"].PutValue(-30);
sheet.Cells["F4"].PutValue(40);
sheet.Cells["G3"].PutValue(-50);
sheet.Cells["G4"].PutValue(60);
// Add data bar conditional formatting
int formatIndex = sheet.ConditionalFormattings.Add();
FormatConditionCollection conds = sheet.ConditionalFormattings[formatIndex];
int idx = conds.AddCondition(FormatConditionType.DataBar);
FormatCondition cond = conds[idx];
// Set up data bar
cond.DataBar.Color = Color.Orange;
cond.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
cond.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
cond.DataBar.ShowValue = false;
// Set data bar border
cond.DataBar.BarBorder.Type = DataBarBorderType.Solid;
cond.DataBar.BarBorder.Color = Color.Plum;
// Set negative bar format
cond.DataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
cond.DataBar.NegativeBarFormat.Color = Color.White;
// Demonstrate BorderColorType property
cond.DataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
cond.DataBar.NegativeBarFormat.BorderColor = Color.Yellow;
// Save the workbook
workbook.Save("NegativeBarFormatBorderColorTypeDemo.xlsx", SaveFormat.Xlsx);
Console.WriteLine("Demo completed. File saved.");
}
}
}
```
### See Also
* enum [DataBarNegativeColorType](../../databarnegativecolortype/)
* class [NegativeBarFormat](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
