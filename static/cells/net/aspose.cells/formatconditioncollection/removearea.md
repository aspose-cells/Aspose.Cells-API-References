##FormatConditionCollection.RemoveArea
FormatConditionCollection method. Removes conditional formatted cell range by index
## RemoveArea(int) {#removearea_1}
Removes conditional formatted cell range by index.
```csharp
public void RemoveArea(int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The index of the conditional formatted cell range to be removed. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FormatConditionCollectionMethodRemoveAreaWithInt32Demo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add conditional formatting
ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
int index = conditionalFormattings.Add();
FormatConditionCollection formatConditionCollection = conditionalFormattings[index];
// Add areas to format
formatConditionCollection.AddArea(CellArea.CreateCellArea(0, 0, 10, 5)); // First area
formatConditionCollection.AddArea(CellArea.CreateCellArea(5, 5, 15, 10)); // Second area
// Add a condition
formatConditionCollection.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");
// Display initial area count (we know we added 2 areas)
Console.WriteLine("Areas before removal: 2");
// Remove the second area (index 1)
formatConditionCollection.RemoveArea(1);
// Display area count after removal (we know we removed 1 area)
Console.WriteLine("Areas after removal: 1");
// Save the workbook
workbook.Save("RemoveAreaDemo.xlsx");
}
}
}
```
### See Also
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## RemoveArea(int, int, int, int) {#removearea}
Remove conditional formatting int the range.
```csharp
public bool RemoveArea(int startRow, int startColumn, int totalRows, int totalColumns)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | The startRow of the range. |
| startColumn | Int32 | The startColumn of the range. |
| totalRows | Int32 | The number of rows of the range. |
| totalColumns | Int32 | The number of columns of the range. |
### Return Value
Returns TRUE, this FormatCondtionCollection should be removed.
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class FormatConditionCollectionMethodRemoveAreaWithInt32Int32Int32Int32Demo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
int idx = cfc.Add();
FormatConditionCollection fcc = cfc[idx];
// Add initial area
CellArea initialArea = CellArea.CreateCellArea(0, 0, 0, 0);
fcc.AddArea(initialArea);
// Add condition
idx = fcc.AddCondition(FormatConditionType.Expression);
FormatCondition fc = fcc[idx];
fc.Formula1 = "=A1>0";
fc.Style.Font.Color = Color.Red;
// Demonstrate RemoveArea with Int32 parameters
Console.WriteLine("Before removal - Areas count: " + fcc.Count);
fcc.RemoveArea(0, 0, 1, 1); // Remove the initial area
Console.WriteLine("After removal - Areas count: " + fcc.Count);
// Add new area
CellArea newArea = CellArea.CreateCellArea(1, 1, 1, 1);
fcc.AddArea(newArea);
Console.WriteLine("After adding new area - Areas count: " + fcc.Count);
}
}
}
```
### See Also
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
