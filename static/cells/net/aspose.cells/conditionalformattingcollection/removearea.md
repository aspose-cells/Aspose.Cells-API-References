##ConditionalFormattingCollection.RemoveArea
ConditionalFormattingCollection method. Remove all conditional formatting in the range
## ConditionalFormattingCollection.RemoveArea method
Remove all conditional formatting in the range.
```csharp
public void RemoveArea(int startRow, int startColumn, int totalRows, int totalColumns)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | The start row of the range. |
| startColumn | Int32 | The start column of the range. |
| totalRows | Int32 | The number of rows of the range. |
| totalColumns | Int32 | The number of columns of the range. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ConditionalFormattingCollectionMethodRemoveAreaWithInt32Int32Int32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Get the conditional formatting collection
ConditionalFormattingCollection cfc = worksheet.ConditionalFormattings;
// Add some conditional formatting rules
int index = cfc.Add();
FormatConditionCollection fcc = cfc[index];
CellArea area = new CellArea();
area.StartRow = 0;
area.StartColumn = 0;
area.EndRow = 5;
area.EndColumn = 5;
fcc.AddArea(area);
try
{
// Call RemoveArea with parameters (Int32, Int32, Int32, Int32)
cfc.RemoveArea(0, 0, 3, 3);
Console.WriteLine("Conditional formatting removed from area (0,0,3,3)");
// Verify the effect by checking count (this would be 0 if all formatting was removed)
Console.WriteLine($"Remaining conditional formatting areas: {fcc.RangeCount}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing RemoveArea method: {ex.Message}");
}
// Save the result
workbook.Save("RemoveAreaWithInt32Demo.xlsx");
}
}
}
```
### See Also
* class [ConditionalFormattingCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
