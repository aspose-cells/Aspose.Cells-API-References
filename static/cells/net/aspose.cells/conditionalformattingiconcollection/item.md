##ConditionalFormattingIconCollection.Item
ConditionalFormattingIconCollection property. Gets the ConditionalFormattingIcon element at the specified index
## ConditionalFormattingIconCollection indexer
Gets the ConditionalFormattingIcon element at the specified index.
```csharp
public ConditionalFormattingIcon this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |
### Return Value
The element at the specified index.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ConditionalFormattingIconCollectionPropertyItemDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
ConditionalFormattingCollection cformattings = sheet.ConditionalFormattings;
int index = cformattings.Add();
FormatConditionCollection fcs = cformattings[index];
fcs.AddArea(new CellArea { StartRow = 0, EndRow = 0, StartColumn = 0, EndColumn = 0 });
fcs.AddArea(new CellArea { StartRow = 1, EndRow = 1, StartColumn = 1, EndColumn = 1 });
int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
FormatCondition cond = fcs[conditionIndex];
cond.IconSet.Type = IconSetType.ArrowsGray3;
// Demonstrate Item property usage
ConditionalFormattingIcon icon = cond.IconSet.CfIcons[0];
icon.Type = IconSetType.Arrows3;
icon.Index = 0;
workbook.Save("ConditionalFormattingIconCollectionDemo.xlsx");
}
}
}
```
### See Also
* class [ConditionalFormattingIcon](../../conditionalformattingicon/)
* class [ConditionalFormattingIconCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
