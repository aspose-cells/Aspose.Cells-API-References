##Class ListColumnCollection
Aspose.Cells.Tables.ListColumnCollection class. Represents A collection of all the ListColumn objects in the specified ListObject object
## ListColumnCollection class
Represents A collection of all the [`ListColumn`](../listcolumn/) objects in the specified ListObject object.
```csharp
public class ListColumnCollection : CollectionBase<ListColumn>
```
## Properties
| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.tables/listcolumncollection/item/) { get; } | Gets the ListColumn by the index. (2 indexers) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
## Methods
| Name | Description |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ListColumn) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ListColumn, IComparer&lt;ListColumn&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ListColumn, IComparer&lt;ListColumn&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ListColumn) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ListColumn[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ListColumn[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ListColumn[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ListColumn&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ListColumn&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ListColumn&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ListColumn&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ListColumn&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ListColumn&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ListColumn&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ListColumn&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ListColumn&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ListColumn&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ListColumn) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ListColumn, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ListColumn, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ListColumn) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ListColumn, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ListColumn, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Tables;
using System;
public class ListColumnCollectionDemo
{
public static void ListColumnCollectionExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Populate the worksheet with some data
for (int i = 0; i < 5; i++)
{
cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
}
for (int row = 1; row < 10; row++)
{
for (int column = 0; column < 5; column++)
{
cells[row, column].PutValue(row * column);
}
}
// Add a ListObject (table) to the worksheet
ListObjectCollection tables = worksheet.ListObjects;
int index = tables.Add(0, 0, 9, 4, true);
ListObject table = tables[index];
// Access the ListColumnCollection of the ListObject
ListColumnCollection listColumns = table.ListColumns;
// Demonstrate accessing properties of ListColumnCollection
Console.WriteLine("Number of columns in the table: " + listColumns.Count);
// Access individual ListColumn by index
ListColumn firstColumn = listColumns[0];
Console.WriteLine("First column name: " + firstColumn.Name);
// Modify the capacity of the ListColumnCollection
listColumns.Capacity = 10;
Console.WriteLine("New capacity of the ListColumnCollection: " + listColumns.Capacity);
// Save the workbook
workbook.Save("ListColumnCollectionExample.xlsx");
}
}
}
```
### See Also
* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ListColumn](../listcolumn/)
* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)
