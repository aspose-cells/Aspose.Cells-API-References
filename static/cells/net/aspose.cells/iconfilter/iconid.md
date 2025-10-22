##IconFilter.IconId
IconFilter property. Gets and sets Zerobased index of an icon in an icon set
## IconFilter.IconId property
Gets and sets Zero-based index of an icon in an icon set.
```csharp
public int IconId { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class IconFilterPropertyIconIdDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate sample data
for (int i = 0; i < 10; i++)
{
worksheet.Cells[i, 0].PutValue(i + 1);
}
// Apply icon set conditional formatting
ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
int index = conditionalFormattings.Add();
FormatConditionCollection formatConditionCollection = conditionalFormattings[index];
int conditionIndex = formatConditionCollection.AddCondition(FormatConditionType.IconSet);
FormatCondition formatCondition = formatConditionCollection[conditionIndex];
formatCondition.IconSet.Type = IconSetType.TrafficLights31;
// Set range using CellArea
CellArea area = new CellArea();
area.StartRow = 0;
area.EndRow = 9;
area.StartColumn = 0;
area.EndColumn = 0;
formatConditionCollection.AddArea(area);
// Create auto filter with icon filter
worksheet.AutoFilter.Range = "A1:A10";
FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
filterColumn.FilterType = FilterType.IconFilter;
// Get existing filter instead of creating new instance
IconFilter iconFilter = (IconFilter)filterColumn.Filter;
iconFilter.IconSetType = IconSetType.TrafficLights31;
iconFilter.IconId = 0;
Console.WriteLine("Current IconId value: " + iconFilter.IconId);
// Modify IconId to filter different icons
iconFilter.IconId = 1;
workbook.Save("PropertyIconIdDemo.xlsx");
}
}
}
```
### See Also
* class [IconFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
