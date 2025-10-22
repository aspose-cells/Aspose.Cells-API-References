##Cells.ClearContents
Cells method. Clears contents of a range
## ClearContents(CellArea) {#clearcontents}
Clears contents of a range.
```csharp
public void ClearContents(CellArea range)
```
| Parameter | Type | Description |
| --- | --- | --- |
| range | CellArea | Range to be cleared. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodClearContentsWithCellAreaDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
Cells cells = sheet.Cells;
// Populate some data in a cell area
CellArea area = new CellArea();
area.StartRow = 0;
area.StartColumn = 0;
area.EndRow = 2;
area.EndColumn = 2;
for (int row = area.StartRow; row <= area.EndRow; row++)
{
for (int col = area.StartColumn; col <= area.EndColumn; col++)
{
cells[row, col].PutValue($"Data_{row}_{col}");
}
}
Console.WriteLine("Before ClearContents:");
PrintCellAreaContents(cells, area);
// Clear contents of the cell area
cells.ClearContents(area);
Console.WriteLine("\nAfter ClearContents:");
PrintCellAreaContents(cells, area);
}
private static void PrintCellAreaContents(Cells cells, CellArea area)
{
for (int row = area.StartRow; row <= area.EndRow; row++)
{
for (int col = area.StartColumn; col <= area.EndColumn; col++)
{
Console.Write(cells[row, col].StringValue + "\t");
}
Console.WriteLine();
}
}
}
}
```
### See Also
* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## ClearContents(int, int, int, int) {#clearcontents_1}
Clears contents of a range.
```csharp
public void ClearContents(int startRow, int startColumn, int endRow, int endColumn)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | Start row index. |
| startColumn | Int32 | Start column index. |
| endRow | Int32 | End row index. |
| endColumn | Int32 | End column index. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodClearContentsWithInt32Int32Int32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Populate some cells with values
cells[0, 0].PutValue("Value A1");
cells[0, 1].PutValue("Value B1");
cells[1, 0].PutValue("Value A2");
cells[1, 1].PutValue("Value B2");
// Display original values
Console.WriteLine("Before ClearContents:");
Console.WriteLine("A1: " + cells[0, 0].StringValue);
Console.WriteLine("B1: " + cells[0, 1].StringValue);
Console.WriteLine("A2: " + cells[1, 0].StringValue);
Console.WriteLine("B2: " + cells[1, 1].StringValue);
// Clear contents of cells in range (0,1) to (1,1)
cells.ClearContents(0, 1, 1, 1);
// Display values after clearing
Console.WriteLine("\nAfter ClearContents(0, 1, 1, 1):");
Console.WriteLine("A1: " + cells[0, 0].StringValue);
Console.WriteLine("B1: " + cells[0, 1].StringValue);
Console.WriteLine("A2: " + cells[1, 0].StringValue);
Console.WriteLine("B2: " + cells[1, 1].StringValue);
// Save the workbook
workbook.Save("ClearContentsDemo.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
