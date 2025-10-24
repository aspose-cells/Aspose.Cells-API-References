##Class DataSorter
Aspose.Cells.DataSorter class. Summary description for DataSorter
## DataSorter class
Summary description for DataSorter.
```csharp
public class DataSorter
```
## Properties
| Name | Description |
| --- | --- |
| [CaseSensitive](../../aspose.cells/datasorter/casesensitive/) { get; set; } | Gets and sets whether case sensitive when comparing string. |
| [HasHeaders](../../aspose.cells/datasorter/hasheaders/) { get; set; } | Represents whether the range has headers. |
| [Key1](../../aspose.cells/datasorter/key1/) { get; set; } | Represents first sorted column index(absolute position, column A is 0, B is 1, ...). |
| [Key2](../../aspose.cells/datasorter/key2/) { get; set; } | Represents second sorted column index(absolute position, column A is 0, B is 1, ...). |
| [Key3](../../aspose.cells/datasorter/key3/) { get; set; } | Represents third sorted column index(absolute position, column A is 0, B is 1, ...). |
| [Keys](../../aspose.cells/datasorter/keys/) { get; } | Gets the key list of data sorter. |
| [Order1](../../aspose.cells/datasorter/order1/) { get; set; } | Represents sort order of the first key. |
| [Order2](../../aspose.cells/datasorter/order2/) { get; set; } | Represents sort order of the second key. |
| [Order3](../../aspose.cells/datasorter/order3/) { get; set; } | Represents sort order of the third key. |
| [SortAsNumber](../../aspose.cells/datasorter/sortasnumber/) { get; set; } | Indicates whether sorting anything that looks like a number. |
| [SortLeftToRight](../../aspose.cells/datasorter/sortlefttoright/) { get; set; } | True means that sorting orientation is from left to right. False means that sorting orientation is from top to bottom. The default value is false. |
## Methods
| Name | Description |
| --- | --- |
| [AddColorKey](../../aspose.cells/datasorter/addcolorkey/)(int, SortOnType, SortOrder, Color) | Adds color sort key. |
| [AddKey](../../aspose.cells/datasorter/addkey/#addkey_1)(int, SortOrder) | Adds sorted column index and sort order. |
| [AddKey](../../aspose.cells/datasorter/addkey/#addkey_2)(int, SortOrder, string) | Adds sorted column index and sort order with custom sort list. |
| [AddKey](../../aspose.cells/datasorter/addkey/#addkey_3)(int, SortOrder, string[]) | Adds sorted column index and sort order with custom sort list. |
| [AddKey](../../aspose.cells/datasorter/addkey/#addkey)(int, SortOnType, SortOrder, object) | Adds sorted column index and sort order with custom sort list. |
| [Clear](../../aspose.cells/datasorter/clear/)() | Clear all settings. |
| [Sort](../../aspose.cells/datasorter/sort/#sort)() | Sort the data in the range. |
| [Sort](../../aspose.cells/datasorter/sort/#sort_1)(Cells, CellArea) | Sort the data of the area. |
| [Sort](../../aspose.cells/datasorter/sort/#sort_2)(Cells, int, int, int, int) | Sorts the data of the area. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class DataSorterDemo
{
public static void DataSorterExample()
{
// Instantiate a new Workbook object
Workbook workbook = new Workbook("DataSorter_original.xlsx");
// Get the workbook DataSorter object
DataSorter sorter = workbook.DataSorter;
// Set the first order for DataSorter object
sorter.Order1 = SortOrder.Descending;
// Define the first key
sorter.Key1 = 0;
// Set the second order for DataSorter object
sorter.Order2 = SortOrder.Ascending;
// Define the second key
sorter.Key2 = 1;
// Create a cells area (range)
CellArea ca = new CellArea
{
StartRow = 0,
StartColumn = 0,
EndRow = 13,
EndColumn = 1
};
// Sort data in the specified data range (A1:B14)
sorter.Sort(workbook.Worksheets[0].Cells, ca);
// Save the excel file
workbook.Save("DataSorterExample.xlsx");
workbook.Save("DataSorterExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
