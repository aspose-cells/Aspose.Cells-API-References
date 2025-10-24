##ConditionalFormattingIcon.Type
ConditionalFormattingIcon property. Gets and sets the icon set type
## ConditionalFormattingIcon.Type property
Gets and sets the icon set type.
```csharp
public IconSetType Type { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ConditionalFormattingIconPropertyTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue(30);
// Add conditional formatting with icon set
ConditionalFormattingCollection cfs = worksheet.ConditionalFormattings;
int index = cfs.Add();
FormatConditionCollection fc = cfs[index];
fc.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 2, EndColumn = 0 });
int conditionIndex = fc.AddCondition(FormatConditionType.IconSet);
FormatCondition condition = fc[conditionIndex];
condition.IconSet.Type = IconSetType.Symbols3;
// Apply formatting and calculate
workbook.CalculateFormula();
// Get formatting result and demonstrate Type property
Cell cell = worksheet.Cells["A2"];
ConditionalFormattingResult formattingResult = cell.GetConditionalFormattingResult();
Console.WriteLine("Icon Set Type: " + formattingResult.ConditionalFormattingIcon.Type);
Console.WriteLine("Icon Index: " + formattingResult.ConditionalFormattingIcon.Index);
}
}
}
```
### See Also
* enum [IconSetType](../../iconsettype/)
* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
