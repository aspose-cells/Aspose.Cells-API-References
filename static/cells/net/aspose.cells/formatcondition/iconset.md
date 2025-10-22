##FormatCondition.IconSet
FormatCondition property. Get the conditional formattings IconSet instance. The default instances IconSetType is TrafficLights31. Valid only for type  IconSet
## FormatCondition.IconSet property
Get the conditional formatting's "IconSet" instance. The default instance's IconSetType is TrafficLights31. Valid only for type = IconSet.
```csharp
public IconSet IconSet { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FormatConditionPropertyIconSetDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
for (int i = 0; i < 10; i++)
{
sheet.Cells[i, 0].PutValue(i * 10);
}
// Add conditional formatting
int index = sheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
// Set the cell range
CellArea area = new CellArea();
area.StartRow = 0;
area.EndRow = 9;
area.StartColumn = 0;
area.EndColumn = 0;
fcs.AddArea(area);
// Add condition and set type to IconSet
int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
FormatCondition condition = fcs[conditionIndex];
// Get the IconSet and configure it
IconSet iconSet = condition.IconSet;
iconSet.Type = IconSetType.TrafficLights31;
iconSet.ShowValue = true;
iconSet.Reverse = false;
// Save the workbook
workbook.Save("IconSetDemo.xlsx");
}
}
}
```
### See Also
* class [IconSet](../../iconset/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
