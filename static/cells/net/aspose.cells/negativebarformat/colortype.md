##NegativeBarFormat.ColorType
NegativeBarFormat property. Gets or sets whether to use the same fill color as positive data bars
## NegativeBarFormat.ColorType property
Gets or sets whether to use the same fill color as positive data bars.
```csharp
public DataBarNegativeColorType ColorType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class NegativeBarFormatPropertyColorTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["E3"].PutValue(-10);
sheet.Cells["E4"].PutValue(20);
sheet.Cells["F3"].PutValue(-15);
sheet.Cells["F4"].PutValue(25);
sheet.Cells["G3"].PutValue(-5);
sheet.Cells["G4"].PutValue(15);
// Create conditional formatting range
CellArea area = new CellArea();
area.StartRow = 2;
area.StartColumn = 4;
area.EndRow = 3;
area.EndColumn = 6;
// Add data bar conditional formatting
int formatIndex = sheet.ConditionalFormattings.Add();
FormatConditionCollection conds = sheet.ConditionalFormattings[formatIndex];
conds.AddArea(area);
int idx = conds.AddCondition(FormatConditionType.DataBar);
FormatCondition cond = conds[idx];
// Set data bar properties
cond.DataBar.Color = Color.Orange;
cond.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
cond.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
// Configure negative bar format
cond.DataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
cond.DataBar.NegativeBarFormat.Color = Color.White;
cond.DataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
cond.DataBar.NegativeBarFormat.BorderColor = Color.Yellow;
// Save the workbook
workbook.Save("NegativeBarFormatDemo.xlsx", SaveFormat.Xlsx);
Console.WriteLine("Demo completed. File saved with negative bar formatting.");
}
}
}
```
### See Also
* enum [DataBarNegativeColorType](../../databarnegativecolortype/)
* class [NegativeBarFormat](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
