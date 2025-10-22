##FormatConditionCollection.Item
FormatConditionCollection property. Gets the formatting condition by index
## FormatConditionCollection indexer
Gets the formatting condition by index.
```csharp
public FormatCondition this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | the index of the formatting condition to return. |
### Return Value
the formatting condition
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FormatConditionCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add a format condition collection
int index = sheet.ConditionalFormattings.Add();
FormatConditionCollection fcc = sheet.ConditionalFormattings[index];
// Add a format condition
fcc.Add(CellArea.CreateCellArea(0, 0, 0, 3),
FormatConditionType.CellValue, OperatorType.Between, "=A1", "=B1");
// Access the first format condition using Item property
FormatCondition condition = fcc[0];
// Display the formulas
Console.WriteLine("Formula1: " + condition.Formula1);
Console.WriteLine("Formula2: " + condition.Formula2);
// Modify the formulas using Item property
fcc[0].Formula1 = "=C1";
fcc[0].Formula2 = "=D1";
// Display modified formulas
Console.WriteLine("Modified Formula1: " + fcc[0].Formula1);
Console.WriteLine("Modified Formula2: " + fcc[0].Formula2);
}
}
}
```
### See Also
* class [FormatCondition](../../formatcondition/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
