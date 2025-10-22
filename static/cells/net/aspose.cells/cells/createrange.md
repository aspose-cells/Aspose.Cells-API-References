##Cells.CreateRange
Cells method. Creates a Range object from a range of cells
## CreateRange(string, string) {#createrange_3}
Creates a [`Range`](../../range/) object from a range of cells.
```csharp
public Range CreateRange(string upperLeftCell, string lowerRightCell)
```
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftCell | String | Upper left cell name. |
| lowerRightCell | String | Lower right cell name. |
### Return Value
A [`Range`](../../range/) object
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodCreateRangeWithStringStringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
// Create a range from A1 to A2
Aspose.Cells.Range range = cells.CreateRange("A1", "A2");
range.Name = "MyRange";
// Set values in the range
cells["A1"].PutValue(10);
cells["A2"].PutValue(20);
// Use the range in a formula
cells["B1"].Formula = "=SUM(MyRange)";
// Calculate the formula
workbook.CalculateFormula();
Console.WriteLine("Sum of MyRange (A1:A2) is: " + cells["B1"].IntValue);
}
}
}
```
### See Also
* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## CreateRange(int, int, int, int) {#createrange_1}
Creates a [`Range`](../../range/) object from a range of cells.
```csharp
public Range CreateRange(int firstRow, int firstColumn, int totalRows, int totalColumns)
```
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | First row of this range |
| firstColumn | Int32 | First column of this range |
| totalRows | Int32 | Number of rows |
| totalColumns | Int32 | Number of columns |
### Return Value
A [`Range`](../../range/) object
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodCreateRangeWithInt32Int32Int32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Create source range (starting row 2, column 2 with 3 rows and 4 columns)
Aspose.Cells.Range rangeSrc = cells.CreateRange(2, 2, 3, 4);
// Fill the source range with sample data
for (int i = 0; i < rangeSrc.RowCount; i++)
{
for (int j = 0; j < rangeSrc.ColumnCount; j++)
{
rangeSrc[i, j].PutValue($"Data {i},{j}");
}
}
// Create destination range (starting row 8, column 0 with same dimensions)
Aspose.Cells.Range rangeDest = cells.CreateRange(8, 0, 3, 4);
// Copy values from source to destination
rangeDest.CopyValue(rangeSrc);
// Save the workbook
workbook.Save("CreateRangeDemo.xlsx");
}
}
}
```
### See Also
* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## CreateRange(string) {#createrange_2}
Creates a [`Range`](../../range/) object from an address of the range.
```csharp
public Range CreateRange(string address)
```
| Parameter | Type | Description |
| --- | --- | --- |
| address | String | The address of the range. |
### Return Value
A [`Range`](../../range/) object
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodCreateRangeWithStringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a range using string address
Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:D4");
// Fill data in the range
for (int i = 0; i < range.RowCount; i++)
{
for (int j = 0; j < range.ColumnCount; j++)
{
range[i, j].PutValue($"Cell {i},{j}");
}
}
// Create another range in a new worksheet
workbook.Worksheets.Add();
Worksheet worksheet2 = workbook.Worksheets[1];
Aspose.Cells.Range range2 = worksheet2.Cells.CreateRange("A1:C3");
// Copy data between ranges
range2.Copy(range);
// Save the workbook
workbook.Save("CreateRangeWithStringDemo.xlsx");
}
}
}
```
### See Also
* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## CreateRange(int, int, bool) {#createrange}
Creates a [`Range`](../../range/) object from rows of cells or columns of cells.
```csharp
public Range CreateRange(int firstIndex, int number, bool isVertical)
```
| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | Int32 | First row index or first column index, zero based. |
| number | Int32 | Total number of rows or columns, one based. |
| isVertical | Boolean | True - Range created from columns of cells. False - Range created from rows of cells. |
### Return Value
A [`Range`](../../range/) object.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodCreateRangeWithInt32Int32BooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Create a range starting from cell A1 (0,0) with 5 rows and 3 columns
Aspose.Cells.Range range = cells.CreateRange(0, 0, true);
// Fill some data into the range
for (int i = 0; i < range.RowCount; i++)
{
for (int j = 0; j < range.ColumnCount; j++)
{
range[i, j].PutValue($"Row {i}, Col {j}");
}
}
// Save the workbook
workbook.Save("CreateRangeDemo.xlsx");
}
}
}
```
### See Also
* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
