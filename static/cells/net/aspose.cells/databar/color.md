##DataBar.Color
DataBar property. Get or set this DataBars Color
## DataBar.Color property
Get or set this DataBar's Color.
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
public class DataBarPropertyColorDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a range of cells
CellArea area = new CellArea();
area.StartRow = 2;
area.StartColumn = 4;
area.EndRow = 3;
area.EndColumn = 6;
// Add some sample data
worksheet.Cells["E3"].PutValue(10);
worksheet.Cells["F3"].PutValue(20);
worksheet.Cells["G3"].PutValue(30);
worksheet.Cells["E4"].PutValue(15);
worksheet.Cells["F4"].PutValue(25);
worksheet.Cells["G4"].PutValue(35);
// Add conditional formatting with data bar
int formatIndex = worksheet.ConditionalFormattings.Add();
FormatConditionCollection conditions = worksheet.ConditionalFormattings[formatIndex];
int index = conditions.AddCondition(FormatConditionType.DataBar);
FormatCondition condition = conditions[index];
// Set data bar properties including Color
condition.DataBar.Color = Color.Orange;
condition.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
condition.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
condition.DataBar.ShowValue = false;
// Set border properties
condition.DataBar.BarBorder.Type = DataBarBorderType.Solid;
condition.DataBar.BarBorder.Color = Color.Plum;
// Set fill type
condition.DataBar.BarFillType = DataBarFillType.Gradient;
// Set axis properties
condition.DataBar.AxisColor = Color.Red;
condition.DataBar.AxisPosition = DataBarAxisPosition.Automatic;
// Set negative bar properties
condition.DataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
condition.DataBar.NegativeBarFormat.Color = Color.White;
condition.DataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
condition.DataBar.NegativeBarFormat.BorderColor = Color.Yellow;
// Apply the formatting to the range
conditions.AddArea(area);
// Save the workbook
workbook.Save("DataBarPropertyColorDemo.xlsx", SaveFormat.Xlsx);
Console.WriteLine("DataBarPropertyColorDemo executed successfully.");
}
}
}
```
### See Also
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
