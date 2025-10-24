##CellArea.CreateCellArea
CellArea method. Creates a cell area
## CreateCellArea(int, int, int, int) {#createcellarea}
Creates a cell area.
```csharp
public static CellArea CreateCellArea(int startRow, int startColumn, int endRow, int endColumn)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | The start row. |
| startColumn | Int32 | The start column. |
| endRow | Int32 | The end row. |
| endColumn | Int32 | The end column. |
### Return Value
Return a [`CellArea`](../).
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellAreaMethodCreateCellAreaWithInt32Int32Int32Int32Demo
{
public static void Run()
{
Workbook wb = new Workbook();
Cells cells = wb.Worksheets[0].Cells;
// Populate cells with sample data
int[] values = { 1, 3, 2, 6, 4, 5, 8, 9, 7 };
for (int i = 0; i < values.Length; i++)
{
cells[i, i / 3].PutValue(values[i]);
}
// Create and configure data sorter
DataSorter sorter = wb.DataSorter;
sorter.Clear();
sorter.Order1 = SortOrder.Ascending;
sorter.Key1 = 2;
sorter.Order2 = SortOrder.Ascending;
sorter.Key2 = 1;
sorter.Order3 = SortOrder.Ascending;
sorter.Key3 = 0;
// Sort using CreateCellArea with Int32 parameters
sorter.Sort(cells, CellArea.CreateCellArea(0, 0, 8, 2));
// Output sorted values
Console.WriteLine("Sorted values:");
for (int i = 0; i < 9; i++)
{
Console.WriteLine(cells[i, 2 - i / 3].IntValue);
}
}
}
}
```
### See Also
* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## CreateCellArea(string, string) {#createcellarea_1}
Creates a cell area.
```csharp
public static CellArea CreateCellArea(string startCellName, string endCellName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startCellName | String | The top-left cell of the range. |
| endCellName | String | The bottom-right cell of the range. |
### Return Value
Return a [`CellArea`](../).
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellAreaMethodCreateCellAreaWithStringStringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
// Populate some data in column A
for (int i = 0; i < 10; i++)
{
cells[i, 0].PutValue($"Data {i}");
}
// Create cell area from B1 to B10
CellArea area = CellArea.CreateCellArea("B1", "B10");
// Insert range shifting cells down
cells.InsertRange(area, ShiftType.Down);
// Verify the operation by checking cell values
Console.WriteLine("Inserted range from B1 to B10. Total rows: " + cells.Rows.Count);
}
}
}
```
### See Also
* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
