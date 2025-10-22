##CellWatchCollection.Add
CellWatchCollection method. Adds CellWatch with row and column
## Add(int, int) {#add}
Adds [`CellWatch`](../../cellwatch/) with row and column.
```csharp
public int Add(int row, int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row index. |
| column | Int32 | The column index. |
### Return Value
Returns the position of this item in the collection.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellWatchCollectionMethodAddWithInt32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Get the CellWatchCollection from the worksheet
CellWatchCollection cellWatchCollection = worksheet.CellWatches;
try
{
// Call the Add method with row and column indices (Int32, Int32)
int index = cellWatchCollection.Add(5, 3); // Adding cell at row 6, column D (0-based)
Console.WriteLine($"CellWatch added at index: {index}");
// Verify the added cell watch
CellWatch cellWatch = cellWatchCollection[index];
Console.WriteLine($"Watching cell: {cellWatch.Row},{cellWatch.Column}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Add method: {ex.Message}");
}
// Save the result
workbook.Save("CellWatchCollectionMethodAddWithInt32Int32Demo.xlsx");
}
}
}
```
### See Also
* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Add(string) {#add_1}
Adds [`CellWatch`](../../cellwatch/) with the name the of cell.
```csharp
public int Add(string cellName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | The name of the cell. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellWatchCollectionMethodAddWithStringDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add some cell watches
worksheet.CellWatches.Add("A1");
worksheet.CellWatches.Add("B2");
worksheet.CellWatches.Add("C3");
// Display count of cell watches
Console.WriteLine("Cell Watches Count: " + worksheet.CellWatches.Count);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
