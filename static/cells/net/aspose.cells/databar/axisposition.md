##DataBar.AxisPosition
DataBar property. Gets or sets the position of the axis of the data bars specified by a conditional formatting rule
## DataBar.AxisPosition property
Gets or sets the position of the axis of the data bars specified by a conditional formatting rule.
```csharp
public DataBarAxisPosition AxisPosition { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DataBarPropertyAxisPositionDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
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
// Configure data bar properties
cond.DataBar.Color = Color.Orange;
cond.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
cond.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
cond.DataBar.ShowValue = false;
// Set axis position (core demonstration)
cond.DataBar.AxisPosition = DataBarAxisPosition.Automatic;
cond.DataBar.AxisColor = Color.Red;
// Save the workbook
workbook.Save("DataBarAxisPositionDemo.xlsx", SaveFormat.Xlsx);
Console.WriteLine("DataBar with AxisPosition demo created successfully.");
}
}
}
```
### See Also
* enum [DataBarAxisPosition](../../databaraxisposition/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
