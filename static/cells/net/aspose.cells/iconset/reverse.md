##IconSet.Reverse
IconSet property. Get or set the flag indicating whether to reverses the default order of the icons in this icon set. Default value is false
## IconSet.Reverse property
Get or set the flag indicating whether to reverses the default order of the icons in this icon set. Default value is false.
```csharp
public bool Reverse { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class IconSetPropertyReverseDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue(30);
worksheet.Cells["A4"].PutValue(40);
worksheet.Cells["A5"].PutValue(50);
// Add conditional formatting
ConditionalFormattingCollection cfs = worksheet.ConditionalFormattings;
int index = cfs.Add();
FormatConditionCollection cf = cfs[index];
// Set the range
CellArea area = new CellArea();
area.StartRow = 0;
area.EndRow = 4;
area.StartColumn = 0;
area.EndColumn = 0;
cf.AddArea(area);
// Create icon set conditional formatting
cf.AddCondition(FormatConditionType.IconSet);
IconSet iconSet = cf[0].IconSet;
// Configure icon set
iconSet.Type = IconSetType.Arrows3;
iconSet.ShowValue = true;
// Demonstrate Reverse property
Console.WriteLine("Original IconSet Reverse value: " + iconSet.Reverse);
iconSet.Reverse = true;
Console.WriteLine("Modified IconSet Reverse value: " + iconSet.Reverse);
// Save the workbook
workbook.Save("IconSetPropertyReverseDemo_out.xlsx");
}
}
}
```
### See Also
* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
