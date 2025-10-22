##IconSet.IsCustom
IconSet property. Indicates whether the icon set is custom. Default value is false
## IconSet.IsCustom property
Indicates whether the icon set is custom. Default value is false.
```csharp
public bool IsCustom { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class IconSetPropertyIsCustomDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
for (int i = 0; i < 10; i++)
{
worksheet.Cells[i, 0].PutValue(i * 10);
}
// Add conditional formatting with custom icon set
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
// Set range for conditional formatting
CellArea area = new CellArea();
area.StartRow = 0;
area.StartColumn = 0;
area.EndRow = 9;
area.EndColumn = 0;
fcs.AddArea(area);
// Add icon set condition
int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
FormatCondition condition = fcs[conditionIndex];
// Set icon set type (using valid IconSetType)
condition.IconSet.Type = IconSetType.TrafficLights31;
// Verify the IsCustom property (read-only)
Console.WriteLine("Is IconSet custom? " + condition.IconSet.IsCustom);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
