##Cells.InsertRange
Cells method. Inserts a range of cells and shift cells according to the shift option
## InsertRange(CellArea, int, ShiftType, bool) {#insertrange_2}
Inserts a range of cells and shift cells according to the shift option.
```csharp
public void InsertRange(CellArea area, int shiftNumber, ShiftType shiftType, bool updateReference)
```
| Parameter | Type | Description |
| --- | --- | --- |
| area | CellArea | Shift area. |
| shiftNumber | Int32 | Number of rows or columns to be inserted. |
| shiftType | ShiftType | Shift cells option. |
| updateReference | Boolean | Indicates whether update references in other worksheets. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodInsertRangeWithCellAreaInt32ShiftTypeBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Populate some sample data
cells["A1"].PutValue("Header");
cells["A2"].PutValue(100);
cells["A3"].PutValue(200);
// Define the area to insert (rows 2-3, column A)
CellArea area = CellArea.CreateCellArea(1, 0, 2, 0);
// Insert range shifting cells right and update references
cells.InsertRange(area, 1, ShiftType.Right, true);
// Verify the operation by checking values
Console.WriteLine("A2 value after insert: " + cells["A2"].StringValue);
Console.WriteLine("B2 value after insert: " + cells["B2"].StringValue);
}
}
}
```
### See Also
* struct [CellArea](../../cellarea/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## InsertRange(CellArea, ShiftType) {#insertrange}
Inserts a range of cells and shift cells according to the shift option.
```csharp
public void InsertRange(CellArea area, ShiftType shiftType)
```
| Parameter | Type | Description |
| --- | --- | --- |
| area | CellArea | Shift area. |
| shiftType | ShiftType | Shift cells option. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodInsertRangeWithCellAreaShiftTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Fill some sample data
for (int row = 0; row < 10; row++)
{
for (int col = 0; col < 5; col++)
{
cells[row, col].PutValue($"R{row}C{col}");
}
}
// Define the cell area to insert
CellArea area = new CellArea();
area.StartRow = 2;
area.EndRow = 4;
area.StartColumn = 1;
area.EndColumn = 3;
// Insert range and shift cells down
cells.InsertRange(area, ShiftType.Down);
// Save the workbook
workbook.Save("InsertRangeDemo.xlsx");
}
}
}
```
### See Also
* struct [CellArea](../../cellarea/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## InsertRange(CellArea, int, ShiftType) {#insertrange_1}
Inserts a range of cells and shift cells according to the shift option.
```csharp
public void InsertRange(CellArea area, int shiftNumber, ShiftType shiftType)
```
| Parameter | Type | Description |
| --- | --- | --- |
| area | CellArea | Shift area. |
| shiftNumber | Int32 | Number of rows or columns to be inserted. |
| shiftType | ShiftType | Shift cells option. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodInsertRangeWithCellAreaInt32ShiftTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data
worksheet.Cells["A1"].PutValue("Original Data");
worksheet.Cells["B1"].PutValue(100);
worksheet.Cells["C1"].PutValue(200);
// Define the cell area to insert (single cell B1)
CellArea area = new CellArea();
area.StartRow = 0;
area.EndRow = 0;
area.StartColumn = 1;
area.EndColumn = 1;
// Insert range shifting cells right
worksheet.Cells.InsertRange(area, 1, ShiftType.Right);
// Save the workbook
workbook.Save("InsertRangeDemo.xlsx");
}
}
}
```
### See Also
* struct [CellArea](../../cellarea/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
