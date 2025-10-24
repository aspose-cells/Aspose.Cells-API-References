##Cells.MinColumn
Cells property. Minimum column index of those cells that have been instantiated in the collectiondoes not include the column where style is defined for the whole column but no cell has been instantiated in it
## Cells.MinColumn property
Minimum column index of those cells that have been instantiated in the collection(does not include the column where style is defined for the whole column but no cell has been instantiated in it).
```csharp
public int MinColumn { get; }
```
### Remarks
This property needs to iterate and check cells and rows dynamically, so it is a time-consumed progress and should not be invoked repeatedly, such as using it directly as condition in a loop.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsPropertyMinColumnDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Access cells collection
Cells cells = worksheet.Cells;
// Populate some data in columns 2, 3 and 4 (B, C, D)
cells["B1"].PutValue("Data in Column B");
cells["C1"].PutValue("Data in Column C");
cells["D1"].PutValue("Data in Column D");
// Get the minimum column index that contains data
int minColumn = cells.MinColumn;
// Get the maximum column index that contains data
int maxColumn = cells.MaxColumn;
Console.WriteLine("Minimum column with data: " + minColumn); // Should output 1 (column B)
Console.WriteLine("Maximum column with data: " + maxColumn); // Should output 3 (column D)
// Clear column B to demonstrate MinColumn change
cells.DeleteColumn(1);
Console.WriteLine("\nAfter deleting column B:");
Console.WriteLine("New minimum column with data: " + cells.MinColumn); // Should now output 2 (column C)
Console.WriteLine("Maximum column with data: " + cells.MaxColumn); // Should still output 3 (column D)
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
