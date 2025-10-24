##FormatConditionCollection.AddArea
FormatConditionCollection method. Adds a conditional formatted cell range
## FormatConditionCollection.AddArea method
Adds a conditional formatted cell range.
```csharp
public int AddArea(CellArea cellArea)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | CellArea | Conditional formatted cell range. |
### Return Value
Conditional formatted cell rang index.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FormatConditionCollectionMethodAddAreaWithCellAreaDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
for (int row = 0; row < 10; row++)
{
for (int col = 0; col < 10; col++)
{
worksheet.Cells[row, col].PutValue(row * col);
}
}
// Add conditional formatting
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection formatCollection = worksheet.ConditionalFormattings[index];
// Create format condition
formatCollection.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");
// Create cell areas and add them to the format collection
CellArea area1 = CellArea.CreateCellArea(0, 0, 4, 4);
CellArea area2 = CellArea.CreateCellArea(5, 5, 9, 9);
formatCollection.AddArea(area1);
formatCollection.AddArea(area2);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* struct [CellArea](../../cellarea/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
