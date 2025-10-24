##ConditionalFormattingIcon.Index
ConditionalFormattingIcon property. Gets and sets the icons index in the icon set
## ConditionalFormattingIcon.Index property
Gets and sets the icon's index in the icon set.
```csharp
public int Index { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ConditionalFormattingIconPropertyIndexDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue(10);
sheet.Cells["A2"].PutValue(20);
sheet.Cells["A3"].PutValue(30);
sheet.Cells["A4"].PutValue(40);
// Add icon set conditional formatting
int index = sheet.ConditionalFormattings.Add();
FormatConditionCollection fcc = sheet.ConditionalFormattings[index];
fcc.AddCondition(FormatConditionType.IconSet);
// Set icon set properties
FormatCondition condition = fcc[0];
condition.IconSet.Type = IconSetType.Arrows3;
ConditionalFormattingIconCollection icons = condition.IconSet.CfIcons;
// Display the index of each icon
Console.WriteLine("Icon Indexes:");
for (int i = 0; i < icons.Count; i++)
{
Console.WriteLine($"Icon {i}: Index = {icons[i].Index}");
}
// Modify and show index property
icons[1].Index = 2;
Console.WriteLine($"Modified Icon 1 Index: {icons[1].Index}");
}
}
}
```
### See Also
* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
