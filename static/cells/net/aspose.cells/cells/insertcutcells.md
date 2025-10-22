##Cells.InsertCutCells
Cells method. Insert cut range
## Cells.InsertCutCells method
Insert cut range.
```csharp
public void InsertCutCells(Range cutRange, int row, int column, ShiftType shiftType)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cutRange | Range | The cut range. |
| row | Int32 | The row. |
| column | Int32 | The column. |
| shiftType | ShiftType | The shift type . |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodInsertCutCellsWithRangeInt32Int32ShiftTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet and its cells
Worksheet sourceSheet = workbook.Worksheets[0];
Cells sourceCells = sourceSheet.Cells;
// Add some data to the source cells
sourceCells["A1"].PutValue("Source A1");
sourceCells["B1"].PutValue("Source B1");
sourceCells["A2"].PutValue("Source A2");
sourceCells["B2"].PutValue("Source B2");
// Create a second worksheet as destination
Worksheet destSheet = workbook.Worksheets.Add("Sheet2");
Cells destCells = destSheet.Cells;
// Add some initial data to destination
destCells["A1"].PutValue("Dest A1");
destCells["B1"].PutValue("Dest B1");
// Create a range to cut (A1:B2 from source sheet)
Aspose.Cells.Range cutRange = sourceCells.CreateRange("A1:B2");
// Insert the cut cells at B2 in destination sheet, shifting cells down
destCells.InsertCutCells(cutRange, 1, 1, ShiftType.Down);
// Save the workbook
workbook.Save("InsertCutCellsDemo.xlsx");
Console.WriteLine("InsertCutCells demo executed successfully.");
}
}
}
```
### See Also
* class [Range](../../range/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
