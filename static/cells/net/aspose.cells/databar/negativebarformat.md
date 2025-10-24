##DataBar.NegativeBarFormat
DataBar property. Gets the NegativeBarFormat object associated with a data bar conditional formatting rule
## DataBar.NegativeBarFormat property
Gets the NegativeBarFormat object associated with a data bar conditional formatting rule.
```csharp
public NegativeBarFormat NegativeBarFormat { get; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DataBarPropertyNegativeBarFormatDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data with negative values
sheet.Cells["E3"].PutValue(-10);
sheet.Cells["E4"].PutValue(20);
sheet.Cells["F3"].PutValue(-30);
sheet.Cells["F4"].PutValue(40);
sheet.Cells["G3"].PutValue(-50);
sheet.Cells["G4"].PutValue(60);
// Add data bar conditional formatting
int formatIndex = sheet.ConditionalFormattings.Add();
FormatConditionCollection conditions = sheet.ConditionalFormattings[formatIndex];
int index = conditions.AddCondition(FormatConditionType.DataBar);
FormatCondition condition = conditions[index];
// Set data bar properties
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
// Configure negative bar format
condition.DataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
condition.DataBar.NegativeBarFormat.Color = Color.White;
condition.DataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
condition.DataBar.NegativeBarFormat.BorderColor = Color.Yellow;
// Save the workbook
workbook.Save("DataBarNegativeFormatDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [NegativeBarFormat](../../negativebarformat/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
