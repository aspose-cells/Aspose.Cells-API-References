##Class DataSorterKey
Aspose.Cells.DataSorterKey class. Represents the key of the data sorter
## DataSorterKey class
Represents the key of the data sorter.
```csharp
public class DataSorterKey
```
## Properties
| Name | Description |
| --- | --- |
| [Color](../../aspose.cells/datasorterkey/color/) { get; } | Gets the sorted color. |
| [IconId](../../aspose.cells/datasorterkey/iconid/) { get; } | Represents the id of the icon set type. |
| [IconSetType](../../aspose.cells/datasorterkey/iconsettype/) { get; } | Represents the icon set type. |
| [Index](../../aspose.cells/datasorterkey/index/) { get; } | Gets the sorted column index(absolute position, column A is 0, B is 1, ...). |
| [Order](../../aspose.cells/datasorterkey/order/) { get; } | Indicates the order of sorting. |
| [Type](../../aspose.cells/datasorterkey/type/) { get; } | Represents the type of sorting. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Drawing;
public class DataSorterKeyDemo
{
public static void DataSorterKeyExample()
{
// Create a workbook object and load a template file
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data to sort
worksheet.Cells["A1"].PutValue("USA");
worksheet.Cells["A2"].PutValue("China");
worksheet.Cells["A3"].PutValue("Brazil");
worksheet.Cells["A4"].PutValue("Russia");
worksheet.Cells["A5"].PutValue("Canada");
// Instantiate data sorter object
DataSorter sorter = workbook.DataSorter;
// Add key for the first column (A) to sort in ascending order
sorter.AddKey(0, SortOrder.Ascending);
// Create a cell area (range) to sort
CellArea ca = CellArea.CreateCellArea("A1", "A5");
// Perform the sort
sorter.Sort(worksheet.Cells, ca);
// Save the output file
workbook.Save("DataSorterKeyExample.xlsx");
workbook.Save("DataSorterKeyExample.pdf");
// Access the DataSorterKeyCollection
DataSorterKeyCollection keys = sorter.Keys;
// Iterate through the keys and print their properties
foreach (DataSorterKey key in keys)
{
Console.WriteLine($"Order: {key.Order}");
Console.WriteLine($"Index: {key.Index}");
Console.WriteLine($"Type: {key.Type}");
Console.WriteLine($"IconSetType: {key.IconSetType}");
Console.WriteLine($"IconId: {key.IconId}");
Console.WriteLine($"Color: {key.Color}");
}
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
