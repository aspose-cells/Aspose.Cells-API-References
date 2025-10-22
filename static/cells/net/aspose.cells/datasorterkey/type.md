##DataSorterKey.Type
DataSorterKey property. Represents the type of sorting
## DataSorterKey.Type property
Represents the type of sorting.
```csharp
public SortOnType Type { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DataSorterKeyPropertyTypeDemo
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
// Create data sorter and add key
DataSorter sorter = workbook.DataSorter;
sorter.AddKey(0, SortOrder.Ascending);
// Sort the data
CellArea ca = CellArea.CreateCellArea("A1", "A5");
sorter.Sort(worksheet.Cells, ca);
// Demonstrate Type property usage
foreach (DataSorterKey key in sorter.Keys)
{
Console.WriteLine($"Key Type: {key.Type}");
}
}
}
}
```
### See Also
* enum [SortOnType](../../sortontype/)
* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
