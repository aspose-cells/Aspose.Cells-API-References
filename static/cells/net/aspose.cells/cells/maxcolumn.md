##Cells.MaxColumn
Cells property. Maximum column index of those cells that have been instantiated in the collectiondoes not include the column where style is defined for the whole column but no cell has been instantiated in it
## Cells.MaxColumn property
Maximum column index of those cells that have been instantiated in the collection(does not include the column where style is defined for the whole column but no cell has been instantiated in it).
```csharp
public int MaxColumn { get; }
```
### Remarks
Return -1 if there is no cell has been instantiated.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsPropertyMaxColumnDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data to cells
worksheet.Cells["A1"].PutValue("Column A");
worksheet.Cells["B1"].PutValue("Column B");
worksheet.Cells["C1"].PutValue("Column C");
// Get the maximum column index with data
int maxColumn = worksheet.Cells.MaxColumn;
Console.WriteLine("Max column with data: " + maxColumn);
// Add data to the next column after max column
worksheet.Cells[0, maxColumn + 1].PutValue("Next Column");
// Verify the new max column
Console.WriteLine("New max column: " + worksheet.Cells.MaxColumn);
// Create another worksheet to demonstrate copying
Worksheet destSheet = workbook.Worksheets.Add("Destination");
// Copy all columns from source to destination
destSheet.Cells.CopyColumns(worksheet.Cells, 0, 0, worksheet.Cells.MaxColumn + 1);
Console.WriteLine("Columns copied successfully");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
