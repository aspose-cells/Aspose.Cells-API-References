##FormatCondition.DataBar
FormatCondition property. Get the conditional formattings DataBar instance. The default instances color is blue. Valid only for type is DataBar
## FormatCondition.DataBar property
Get the conditional formatting's "DataBar" instance. The default instance's color is blue. Valid only for type is DataBar.
```csharp
public DataBar DataBar { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FormatConditionPropertyDataBarDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
for (int i = 0; i < 10; i++)
{
worksheet.Cells[i, 0].PutValue(i + 1);
}
// Add data bar conditional formatting
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
// Set the range for conditional formatting
CellArea area = new CellArea();
area.StartRow = 0;
area.EndRow = 9;
area.StartColumn = 0;
area.EndColumn = 0;
fcs.AddArea(area);
// Add data bar condition and set properties
int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
FormatCondition condition = fcs[conditionIndex];
// Configure DataBar properties
DataBar dataBar = condition.DataBar;
dataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
dataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
dataBar.Color = System.Drawing.Color.Green;
// Save the workbook
workbook.Save("DataBarExample.xlsx");
}
}
}
```
### See Also
* class [DataBar](../../databar/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
