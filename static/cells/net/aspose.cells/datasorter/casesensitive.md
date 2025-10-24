##DataSorter.CaseSensitive
DataSorter property. Gets and sets whether case sensitive when comparing string
## DataSorter.CaseSensitive property
Gets and sets whether case sensitive when comparing string.
```csharp
public bool CaseSensitive { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DataSorterPropertyCaseSensitiveDemo
{
public static void Run()
{
// Create a workbook and worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Add sample data with case variations
cells["A1"].PutValue("apple");
cells["A2"].PutValue("Orange");
cells["A3"].PutValue("banana");
cells["A4"].PutValue("APPLE");
cells["A5"].PutValue("orange");
cells["A6"].PutValue("Banana");
// Create data sorter
DataSorter sorter = workbook.DataSorter;
sorter.Key1 = 0; // Sort by first column
sorter.Order1 = SortOrder.Ascending;
// Demonstrate case-sensitive sorting
Console.WriteLine("Sorting with CaseSensitive = true:");
sorter.CaseSensitive = true;
sorter.Sort(cells, CellArea.CreateCellArea("A1", "A6"));
PrintSortedData(cells, "A1:A6");
// Demonstrate case-insensitive sorting
Console.WriteLine("\nSorting with CaseSensitive = false:");
sorter.CaseSensitive = false;
sorter.Sort(cells, CellArea.CreateCellArea("A1", "A6"));
PrintSortedData(cells, "A1:A6");
}
private static void PrintSortedData(Cells cells, string range)
{
Console.WriteLine("Sorted data:");
foreach (Cell cell in cells.CreateRange(range))
{
Console.WriteLine(cell.StringValue);
}
}
}
}
```
### See Also
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
