##ConditionalFormattingCollection.Item
ConditionalFormattingCollection property. Gets the FormatConditions element at the specified index
## ConditionalFormattingCollection indexer
Gets the FormatConditions element at the specified index.
```csharp
public FormatConditionCollection this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ConditionalFormattingCollectionPropertyItemDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue(10);
sheet.Cells["A2"].PutValue(20);
sheet.Cells["A3"].PutValue(30);
// Add conditional formatting
int index = sheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
fcs.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 2, EndColumn = 0 });
// Add format condition
int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "5", "50");
FormatCondition fc = fcs[conditionIndex];
fc.Style.BackgroundColor = System.Drawing.Color.Yellow;
// Access and demonstrate Item property usage
FormatConditionCollection firstFormatting = sheet.ConditionalFormattings[0];
Console.WriteLine($"First formatting has {firstFormatting.Count} conditions");
Console.WriteLine($"First condition operator: {firstFormatting[0].Operator}");
}
}
}
```
### See Also
* class [FormatConditionCollection](../../formatconditioncollection/)
* class [ConditionalFormattingCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
