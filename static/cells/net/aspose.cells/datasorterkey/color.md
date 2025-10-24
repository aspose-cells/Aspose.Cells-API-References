##DataSorterKey.Color
DataSorterKey property. Gets the sorted color
## DataSorterKey.Color property
Gets the sorted color.
```csharp
public Color Color { get; }
```
### Remarks
Only takes effect when [`Type`](../type/) is CellColor or FontColor.
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class DataSorterKeyPropertyColorDemo
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
// Output the color property from keys
foreach (DataSorterKey k in sorter.Keys)
{
Console.WriteLine($"Color: {k.Color}");
}
}
}
}
```
### See Also
* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
