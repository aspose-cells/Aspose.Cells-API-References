##NegativeBarFormat.Color
NegativeBarFormat property. Gets or sets a FormatColor object that you can use to specify the fill color for negative data bars
## NegativeBarFormat.Color property
Gets or sets a FormatColor object that you can use to specify the fill color for negative data bars.
```csharp
public Color Color { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class NegativeBarFormatPropertyColorDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["E3"].PutValue(-10);
sheet.Cells["E4"].PutValue(20);
sheet.Cells["F3"].PutValue(-30);
sheet.Cells["F4"].PutValue(40);
sheet.Cells["G3"].PutValue(-50);
sheet.Cells["G4"].PutValue(60);
// Create conditional formatting
int formatIndex = sheet.ConditionalFormattings.Add();
FormatConditionCollection conds = sheet.ConditionalFormattings[formatIndex];
int idx = conds.AddCondition(FormatConditionType.DataBar);
FormatCondition cond = conds[idx];
// Set up data bar properties
cond.DataBar.Color = Color.Orange;
cond.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
cond.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
cond.DataBar.ShowValue = false;
// Set up negative bar format
cond.DataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
cond.DataBar.NegativeBarFormat.Color = Color.White;
cond.DataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
cond.DataBar.NegativeBarFormat.BorderColor = Color.Yellow;
// Save the workbook
workbook.Save("NegativeBarFormatColorDemo.xlsx", SaveFormat.Xlsx);
Console.WriteLine("NegativeBarFormatPropertyColorDemo executed successfully.");
}
}
}
```
### See Also
* class [NegativeBarFormat](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
