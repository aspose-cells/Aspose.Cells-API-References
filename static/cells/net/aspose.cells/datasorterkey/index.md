##DataSorterKey.Index
DataSorterKey property. Gets the sorted column indexabsolute position column A is 0 B is 1
## DataSorterKey.Index property
Gets the sorted column index(absolute position, column A is 0, B is 1, ...).
```csharp
public int Index { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DataSorterKeyPropertyIndexDemo
{
public static void Run()
{
// Create a workbook object
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to sort
worksheet.Cells["A1"].PutValue("USA");
worksheet.Cells["A2"].PutValue("China");
worksheet.Cells["A3"].PutValue("Brazil");
worksheet.Cells["A4"].PutValue("Russia");
worksheet.Cells["A5"].PutValue("Canada");
// Create data sorter and add sort key
DataSorter sorter = workbook.DataSorter;
sorter.AddKey(0, SortOrder.Ascending);
// Sort the data
CellArea ca = CellArea.CreateCellArea("A1", "A5");
sorter.Sort(worksheet.Cells, ca);
// Demonstrate Index property usage
foreach (DataSorterKey key in sorter.Keys)
{
Console.WriteLine($"Column index being sorted: {key.Index}");
}
// Save the result
workbook.Save("DataSorterKeyExample.xlsx");
}
}
}
```
### See Also
* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
