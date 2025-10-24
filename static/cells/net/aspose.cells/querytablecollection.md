##Class QueryTableCollection
Aspose.Cells.QueryTableCollection class. A collection of QueryTableCollection objects that represent QueryTable collection information
## QueryTableCollection class
A collection of `QueryTableCollection` objects that represent QueryTable collection information.
```csharp
public class QueryTableCollection : CollectionBase<QueryTable>
```
## Properties
| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/querytablecollection/item/) { get; } | Gets the querytable by the specific index. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
## Methods
| Name | Description |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(QueryTable) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(QueryTable, IComparer&lt;QueryTable&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, QueryTable, IComparer&lt;QueryTable&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(QueryTable) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(QueryTable[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(QueryTable[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, QueryTable[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;QueryTable&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;QueryTable&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;QueryTable&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;QueryTable&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;QueryTable&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;QueryTable&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;QueryTable&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;QueryTable&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;QueryTable&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;QueryTable&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(QueryTable) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(QueryTable, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(QueryTable, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(QueryTable) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(QueryTable, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(QueryTable, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class QueryTableCollectionDemo
{
public static void QueryTableCollectionExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet in the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Access the QueryTableCollection of the worksheet
QueryTableCollection queryTables = worksheet.QueryTables;
// Display the count of QueryTables in the worksheet
Console.WriteLine("Number of QueryTables: " + queryTables.Count);
// Set the capacity of the QueryTableCollection
queryTables.Capacity = 10;
Console.WriteLine("Capacity of QueryTableCollection: " + queryTables.Capacity);
// Assuming there is at least one QueryTable, access the first QueryTable
if (queryTables.Count > 0)
{
QueryTable queryTable = queryTables[0];
Console.WriteLine("First QueryTable accessed.");
}
else
{
Console.WriteLine("No QueryTables found in the worksheet.");
}
// Save the workbook
workbook.Save("QueryTableCollectionExample.xlsx");
}
}
}
```
### See Also
* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [QueryTable](../querytable/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
