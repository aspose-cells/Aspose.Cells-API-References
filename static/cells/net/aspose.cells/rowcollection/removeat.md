##RowCollection.RemoveAt
RowCollection method. Remove the row item at the specified indexposition in this collection
## RowCollection.RemoveAt method
Remove the row item at the specified index(position) in this collection.
```csharp
public void RemoveAt(int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | zero-based index(position, not [`Index`](../../row/index/)) of the existing row item in this collection. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class RowCollectionMethodRemoveAtWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data to cells in the first few rows
worksheet.Cells["A1"].PutValue("Row 1");
worksheet.Cells["A2"].PutValue("Row 2");
worksheet.Cells["A3"].PutValue("Row 3");
worksheet.Cells["A4"].PutValue("Row 4");
// Display initial row count
Console.WriteLine($"Initial row count: {worksheet.Cells.Rows.Count}");
try
{
// Call the RemoveAt method to remove row at index 1 (second row)
worksheet.Cells.Rows.RemoveAt(1);
Console.WriteLine("Method executed successfully. Row at index 1 removed.");
// Display updated row count
Console.WriteLine($"Updated row count: {worksheet.Cells.Rows.Count}");
// Show the effect - Row 2 should be removed, Row 3 becomes Row 2
Console.WriteLine("Cell A1: " + worksheet.Cells["A1"].StringValue);
Console.WriteLine("Cell A2: " + worksheet.Cells["A2"].StringValue);
Console.WriteLine("Cell A3: " + worksheet.Cells["A3"].StringValue);
}
catch (Exception ex)
{
Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
}
// Save the result
workbook.Save("RowCollectionMethodRemoveAtWithInt32Demo.xlsx");
}
}
}
```
### See Also
* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
