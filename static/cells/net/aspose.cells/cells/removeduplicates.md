##Cells.RemoveDuplicates
Cells method. Removes duplicate rows in the sheet
## RemoveDuplicates() {#removeduplicates}
Removes duplicate rows in the sheet.
```csharp
public void RemoveDuplicates()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodRemoveDuplicatesDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Cells cells = wb.Worksheets[0].Cells;
// Populate cells with some duplicate values
for (int i = 0; i < 10; i++)
{
for (int j = 0; j < 5; j++)
{
// Create duplicates in every other row
cells[i, j].PutValue(i % 2 == 0 ? "Duplicate" : $"Unique_{i}_{j}");
}
}
Console.WriteLine($"Before RemoveDuplicates: {cells.Count} cells");
// Remove duplicate values
cells.RemoveDuplicates();
Console.WriteLine($"After RemoveDuplicates: {cells.Count} cells");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## RemoveDuplicates(int, int, int, int) {#removeduplicates_1}
Removes duplicate values in the range.
```csharp
public void RemoveDuplicates(int startRow, int startColumn, int endRow, int endColumn)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | The start row. |
| startColumn | Int32 | The start column |
| endRow | Int32 | The end row index. |
| endColumn | Int32 | The end column index. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodRemoveDuplicatesWithInt32Int32Int32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Add sample data with duplicates
cells["A1"].PutValue("Apple");
cells["A2"].PutValue("Orange");
cells["A3"].PutValue("Apple");
cells["A4"].PutValue("Banana");
cells["A5"].PutValue("Orange");
// Remove duplicates from column A (0-based index)
cells.RemoveDuplicates(0, 0, 5, 0);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## RemoveDuplicates(int, int, int, int, bool, int[]) {#removeduplicates_2}
Removes duplicate data of the range.
```csharp
public void RemoveDuplicates(int startRow, int startColumn, int endRow, int endColumn,
bool hasHeaders, int[] columnOffsets)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | The start row. |
| startColumn | Int32 | The start column |
| endRow | Int32 | The end row index. |
| endColumn | Int32 | The end column index. |
| hasHeaders | Boolean | Indicates whether the range contains headers. |
| columnOffsets | Int32[] | The column offsets. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsMethodRemoveDuplicatesWithInt32Int32Int32Int32BooleanIntDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Populate sample data with duplicates
cells[0, 0].PutValue("ID");
cells[0, 1].PutValue("Name");
cells[0, 2].PutValue("Age");
cells[1, 0].PutValue(1);
cells[1, 1].PutValue("John");
cells[1, 2].PutValue(30);
cells[2, 0].PutValue(2);
cells[2, 1].PutValue("Jane");
cells[2, 2].PutValue(25);
cells[3, 0].PutValue(1); // Duplicate ID
cells[3, 1].PutValue("John"); // Duplicate Name
cells[3, 2].PutValue(35);
cells[4, 0].PutValue(3);
cells[4, 1].PutValue("Bob");
cells[4, 2].PutValue(40);
try
{
// Remove duplicates from rows 1-4 (0-based), columns 0-2
// Check duplicates based on first two columns (ID and Name)
cells.RemoveDuplicates(1, 0, 4, 2, true, new int[] { 0, 1 });
Console.WriteLine("Duplicates removed successfully. Remaining rows: " + (cells.MaxDataRow + 1));
}
catch (Exception ex)
{
Console.WriteLine($"Error executing RemoveDuplicates method: {ex.Message}");
}
// Save the result
workbook.Save("RemoveDuplicatesDemo.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
