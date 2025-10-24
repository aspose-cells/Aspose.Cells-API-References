##DataBarBorder.Color
DataBarBorder property. Gets or sets the borders color of data bars specified by a conditional formatting rule
## DataBarBorder.Color property
Gets or sets the border's color of data bars specified by a conditional formatting rule.
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
public class DataBarBorderPropertyColorDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Create a format condition collection
int formatIndex = sheet.ConditionalFormattings.Add();
FormatConditionCollection conds = sheet.ConditionalFormattings[formatIndex];
conds.AddArea(new CellArea { StartRow = 2, StartColumn = 4, EndRow = 3, EndColumn = 6 });
// Add data bar format condition
int idx = conds.AddCondition(FormatConditionType.DataBar);
FormatCondition cond = conds[idx];
// Set data bar properties
cond.DataBar.Color = Color.Orange;
cond.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
cond.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
cond.DataBar.ShowValue = false;
// Set border properties (demonstrating Color usage)
cond.DataBar.BarBorder.Type = DataBarBorderType.Solid;
cond.DataBar.BarBorder.Color = Color.Plum;
// Save the workbook
workbook.Save("DataBarBorderColorDemo.xlsx", SaveFormat.Xlsx);
Console.WriteLine("DataBar border color demo completed.");
}
}
}
```
### See Also
* class [DataBarBorder](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
