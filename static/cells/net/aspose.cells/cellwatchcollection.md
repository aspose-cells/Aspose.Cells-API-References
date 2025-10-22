##Class CellWatchCollection
Aspose.Cells.CellWatchCollection class. Represents the collection of cells on this worksheet being watched in the watch window
## CellWatchCollection class
Represents the collection of cells on this worksheet being watched in the 'watch window'.
```csharp
public class CellWatchCollection : CollectionBase<CellWatch>
```
## Constructors
| Name | Description |
| --- | --- |
| [CellWatchCollection](cellwatchcollection/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/cellwatchcollection/item/) { get; } | Gets and sets [`CellWatch`](../cellwatch/) by index. (2 indexers) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
## Methods
| Name | Description |
| --- | --- |
| [Add](../../aspose.cells/cellwatchcollection/add/#add_1)(string) | Adds [`CellWatch`](../cellwatch/) with the name the of cell. |
| [Add](../../aspose.cells/cellwatchcollection/add/#add)(int, int) | Adds [`CellWatch`](../cellwatch/) with row and column. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(CellWatch) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(CellWatch, IComparer&lt;CellWatch&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, CellWatch, IComparer&lt;CellWatch&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(CellWatch) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(CellWatch[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(CellWatch[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, CellWatch[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;CellWatch&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;CellWatch&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;CellWatch&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;CellWatch&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;CellWatch&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;CellWatch&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;CellWatch&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;CellWatch&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;CellWatch&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;CellWatch&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CellWatch) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CellWatch, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CellWatch, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CellWatch) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CellWatch, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CellWatch, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellWatchCollectionDemo
{
public static void CellWatchCollectionExample()
{
// Instantiating a Workbook object
Workbook workbook = new Workbook();
// Get the first Worksheet
Worksheet sheet = workbook.Worksheets[0];
// Add Cell Watch Item into the watch window
int watchIndex = sheet.CellWatches.Add("B2");
// Access the CellWatchCollection
CellWatchCollection cellWatches = sheet.CellWatches;
// Access the added CellWatch item
CellWatch cellWatch = cellWatches[watchIndex];
// Display the properties of the CellWatch item
Console.WriteLine("Cell Watch Details:");
Console.WriteLine($"Row: {cellWatch.Row}");
Console.WriteLine($"Column: {cellWatch.Column}");
Console.WriteLine($"Cell Name: {cellWatch.CellName}");
// Modify the properties of the CellWatch item
cellWatch.Row = 1;
cellWatch.Column = 1;
cellWatch.CellName = "A2";
// Display the modified properties of the CellWatch item
Console.WriteLine("Modified Cell Watch Details:");
Console.WriteLine($"Row: {cellWatch.Row}");
Console.WriteLine($"Column: {cellWatch.Column}");
Console.WriteLine($"Cell Name: {cellWatch.CellName}");
// Save the workbook
workbook.Save("CellWatchCollectionExample.xlsx");
workbook.Save("CellWatchCollectionExample.pdf");
}
}
}
```
### See Also
* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [CellWatch](../cellwatch/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
