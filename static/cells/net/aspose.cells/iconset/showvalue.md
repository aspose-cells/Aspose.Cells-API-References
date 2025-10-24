##IconSet.ShowValue
IconSet property. Get or set the flag indicating whether to show the values of the cells on which this icon set is applied. Default value is true
## IconSet.ShowValue property
Get or set the flag indicating whether to show the values of the cells on which this icon set is applied. Default value is true.
```csharp
public bool ShowValue { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class IconSetPropertyShowValueDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue(10);
sheet.Cells["A2"].PutValue(20);
sheet.Cells["A3"].PutValue(30);
sheet.Cells["A4"].PutValue(40);
sheet.Cells["A5"].PutValue(50);
// Add icon set conditional formatting
int formatIndex = sheet.ConditionalFormattings.Add();
FormatConditionCollection formatConditions = sheet.ConditionalFormattings[formatIndex];
int index = formatConditions.AddCondition(FormatConditionType.IconSet);
FormatCondition condition = formatConditions[index];
// Set icon set properties
condition.IconSet.Type = IconSetType.TrafficLights31;
condition.IconSet.ShowValue = false; // This hides cell values and shows only icons
condition.IconSet.Reverse = false;
// Set the range for the conditional formatting
CellArea area = new CellArea();
area.StartRow = 0;
area.StartColumn = 0;
area.EndRow = 4;
area.EndColumn = 0;
formatConditions.AddArea(area);
// Save the workbook
workbook.Save("IconSetShowValueDemo.xlsx", SaveFormat.Xlsx);
Console.WriteLine("Workbook saved with icon set conditional formatting (ShowValue = false).");
}
}
}
```
### See Also
* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
