##Class DataSorterKeyCollection
Aspose.Cells.DataSorterKeyCollection class. Represents the key list of data sorter
## DataSorterKeyCollection class
Represents the key list of data sorter.
```csharp
public class DataSorterKeyCollection : CollectionBase<DataSorterKey>
```
## Constructors
| Name | Description |
| --- | --- |
| [DataSorterKeyCollection](datasorterkeycollection/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/datasorterkeycollection/item/) { get; } | Gets and sets [`DataSorterKey`](../datasorterkey/) by index. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
## Methods
| Name | Description |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(DataSorterKey) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(DataSorterKey, IComparer&lt;DataSorterKey&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, DataSorterKey, IComparer&lt;DataSorterKey&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(DataSorterKey) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(DataSorterKey[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(DataSorterKey[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, DataSorterKey[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;DataSorterKey&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;DataSorterKey&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;DataSorterKey&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;DataSorterKey&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;DataSorterKey&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;DataSorterKey&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;DataSorterKey&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;DataSorterKey&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;DataSorterKey&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;DataSorterKey&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DataSorterKey) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DataSorterKey, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DataSorterKey, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DataSorterKey) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DataSorterKey, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DataSorterKey, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class DataSorterKeyCollectionDemo
{
public static void DataSorterKeyCollectionExample()
{
// Instantiate a new Workbook object
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data to the worksheet
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Score");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(85);
worksheet.Cells["A3"].PutValue("Jane");
worksheet.Cells["B3"].PutValue(90);
worksheet.Cells["A4"].PutValue("Doe");
worksheet.Cells["B4"].PutValue(80);
// Get the workbook's DataSorter object
DataSorter sorter = workbook.DataSorter;
// Set the first order for the DataSorter object
sorter.Order1 = Aspose.Cells.SortOrder.Descending;
// Define the first key
sorter.Key1 = 1; // Sorting by the second column (Score)
// Create a cells area (range)
CellArea ca = new CellArea
{
StartRow = 1,
StartColumn = 0,
EndRow = 3,
EndColumn = 1
};
// Sort data in the specified data range (A2:B4)
sorter.Sort(worksheet.Cells, ca);
// Access the DataSorterKeyCollection
DataSorterKeyCollection keys = sorter.Keys;
// Display the count of keys
Console.WriteLine("Number of keys: " + keys.Count);
// Access the first key and display its properties
DataSorterKey key = keys[0];
Console.WriteLine("Key Index: " + key.Index);
Console.WriteLine("Key Order: " + key.Order);
// Save the workbook
workbook.Save("DataSorterKeyCollectionExample.xlsx");
workbook.Save("DataSorterKeyCollectionExample.pdf");
return;
}
}
}
```
### See Also
* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [DataSorterKey](../datasorterkey/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
