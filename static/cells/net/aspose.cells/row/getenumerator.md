##Row.GetEnumerator
Row method. Gets the cells enumerator
## GetEnumerator() {#getenumerator}
Gets the cells enumerator
```csharp
public IEnumerator GetEnumerator()
```
### Return Value
The cells enumerator which will traverse all existing cells in this row.
### Examples
```csharp
using System;
using System.Collections;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RowMethodGetEnumeratorDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Populate some sample data
cells["A1"].PutValue("Name");
cells["B1"].PutValue("Age");
cells["A2"].PutValue("John");
cells["B2"].PutValue(30);
cells["A3"].PutValue("Alice");
cells["B3"].PutValue(25);
// Get enumerator for the first row (header row)
IEnumerator en = cells.Rows[0].GetEnumerator();
while (en.MoveNext())
{
Cell cell = (Cell)en.Current;
Console.WriteLine(cell.Name + ": " + cell.Value);
}
}
}
}
```
### See Also
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## GetEnumerator(bool, bool) {#getenumerator_1}
Gets an enumerator that iterates cells through this row.
```csharp
public IEnumerator GetEnumerator(bool reversed, bool sync)
```
| Parameter | Type | Description |
| --- | --- | --- |
| reversed | Boolean | whether enumerate cells in reversed order |
| sync | Boolean | whether the returned enumerator should check the modification of cells in this row and keep synchronized with it. |
### Return Value
The cells enumerator which will traverse all existing cells in this row.
### Remarks
If the row will be modified(by operations that may cause new Cell be instantiated or existing Cell be removed) during the traversal with the enumerator, synchronized enumerator should be used instead of normal enumerator so that the traversal can continue from the position just after the one has been traversed by the last MoveNext(). However, together with the advantage that no element be skipped or traversed repeatedly, the disadvantage for synchronized enumerator is that the performance will be degraded a bit when comparing with normal enumerator.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Collections;
public class RowMethodGetEnumeratorWithBooleanBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data to cells in the first row
Row row = worksheet.Cells.Rows[0];
worksheet.Cells["A1"].PutValue("Cell A1");
worksheet.Cells["B1"].PutValue("Cell B1");
worksheet.Cells["C1"].PutValue("Cell C1");
try
{
// Call GetEnumerator with reversed=false and sync=true
IEnumerator enumerator = row.GetEnumerator(false, true);
Console.WriteLine("Cells in row 1:");
while (enumerator.MoveNext())
{
Cell cell = (Cell)enumerator.Current;
if (cell != null)
{
Console.WriteLine($"Cell {cell.Name}: {cell.Value}");
}
}
// Call GetEnumerator with reversed=true and sync=false to demonstrate reverse iteration
Console.WriteLine("\nCells in row 1 (reversed order):");
enumerator = row.GetEnumerator(true, false);
while (enumerator.MoveNext())
{
Cell cell = (Cell)enumerator.Current;
if (cell != null)
{
Console.WriteLine($"Cell {cell.Name}: {cell.Value}");
}
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetEnumerator method: {ex.Message}");
}
// Save the workbook
workbook.Save("RowMethodGetEnumeratorWithBooleanBooleanDemo.xlsx");
}
}
}
```
### See Also
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
