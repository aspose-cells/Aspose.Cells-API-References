##Cell.Equals
Cell method. Checks whether this object refers to the same cell with another
## Equals(object) {#equals_1}
Checks whether this object refers to the same cell with another.
```csharp
public override bool Equals(object obj)
```
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | another object |
### Return Value
true if two objects refers to the same cell.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellMethodEqualsWithObjectDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access cells from different locations
Cell cellA1 = worksheet.Cells["A1"];
Cell anotherCellA1 = worksheet.Cells[0, 0]; // Same physical cell as A1
Cell cellB1 = worksheet.Cells["B1"];
// Set identical values in different cells
cellA1.PutValue("Aspose.Cells");
cellB1.PutValue("Aspose.Cells");
try
{
// Compare same physical cell references
bool sameCellComparison = cellA1.Equals(anotherCellA1);
Console.WriteLine($"Same cell comparison: {sameCellComparison}"); // True
// Compare different cells with identical content
bool differentCellComparison = cellA1.Equals(cellB1);
Console.WriteLine($"Different cell comparison: {differentCellComparison}"); // False
// Compare cell with non-cell object
bool invalidTypeComparison = cellA1.Equals("Aspose.Cells");
Console.WriteLine($"Invalid type comparison: {invalidTypeComparison}"); // False
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Equals method: {ex.Message}");
}
// Save the workbook
workbook.Save("CellMethodEqualsWithObjectDemo.xlsx");
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Equals(Cell) {#equals}
Checks whether this object refers to the same cell with another cell object.
```csharp
public bool Equals(Cell cell)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cell | Cell | another cell object |
### Return Value
true if two cell objects refers to the same cell.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellMethodEqualsWithCellDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create cells in different locations (A1 and B1)
Cell cellA1 = worksheet.Cells[0, 0];
Cell cellB1 = worksheet.Cells[0, 1];
// Set identical values in both cells
cellA1.Value = "Aspose.Cells Comparison";
cellB1.Value = "Aspose.Cells Comparison";
try
{
// Compare cellA1 with cellB1 (different locations)
bool equalsResult = cellA1.Equals(cellB1);
Console.WriteLine($"Cell A1 equals Cell B1: {equalsResult}");
// Compare cellA1 with itself (same instance)
equalsResult = cellA1.Equals(cellA1);
Console.WriteLine($"Cell A1 equals itself: {equalsResult}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Equals method: {ex.Message}");
}
// Save the workbook
workbook.Save("CellMethodEqualsWithCellDemo.xlsx");
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
