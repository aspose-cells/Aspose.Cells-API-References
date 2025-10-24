##DataSorter.Keys
DataSorter property. Gets the key list of data sorter
## DataSorter.Keys property
Gets the key list of data sorter.
```csharp
public DataSorterKeyCollection Keys { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DataSorterPropertyKeysDemo
{
public static void Run()
{
// Create a workbook object
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("USA");
worksheet.Cells["A2"].PutValue("China");
worksheet.Cells["A3"].PutValue("Brazil");
worksheet.Cells["A4"].PutValue("Russia");
worksheet.Cells["A5"].PutValue("Canada");
// Initialize data sorter
DataSorter sorter = workbook.DataSorter;
// Add sort key for column A (index 0)
sorter.AddKey(0, SortOrder.Ascending);
// Sort the data
sorter.Sort(worksheet.Cells, CellArea.CreateCellArea("A1", "A5"));
// Demonstrate Keys property usage
DataSorterKeyCollection keys = sorter.Keys;
Console.WriteLine("Sort Keys Information:");
foreach (DataSorterKey key in keys)
{
Console.WriteLine($"Column Index: {key.Index}, Sort Order: {key.Order}");
}
// Save the workbook
workbook.Save("DataSorterKeysDemo.xlsx");
}
}
}
```
### See Also
* class [DataSorterKeyCollection](../../datasorterkeycollection/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
