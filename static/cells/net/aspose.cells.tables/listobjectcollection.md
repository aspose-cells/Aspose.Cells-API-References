##Class ListObjectCollection
Aspose.Cells.Tables.ListObjectCollection class. Represents a collection of ListObject objects in the worksheet
## ListObjectCollection class
Represents a collection of [`ListObject`](../listobject/) objects in the worksheet.
```csharp
public class ListObjectCollection : CollectionBase<ListObject>
```
## Properties
| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.tables/listobjectcollection/item/) { get; } | Gets the ListObject by index. (2 indexers) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
## Methods
| Name | Description |
| --- | --- |
| [Add](../../aspose.cells.tables/listobjectcollection/add/#add_1)(string, string, bool) | Adds a ListObject to the worksheet. |
| [Add](../../aspose.cells.tables/listobjectcollection/add/#add)(int, int, int, int, bool) | Adds a ListObject to the worksheet. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ListObject) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ListObject, IComparer&lt;ListObject&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ListObject, IComparer&lt;ListObject&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ListObject) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ListObject[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ListObject[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ListObject[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ListObject&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ListObject&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ListObject&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ListObject&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ListObject&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ListObject&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ListObject&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ListObject&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ListObject&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ListObject&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ListObject) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ListObject, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ListObject, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ListObject) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ListObject, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ListObject, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
| [UpdateColumnName](../../aspose.cells.tables/listobjectcollection/updatecolumnname/)() | Update all column name of the tables. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Tables;
using System;
public class ListObjectCollectionDemo
{
public static void ListObjectCollectionExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Access the ListObjectCollection of the worksheet
ListObjectCollection listObjects = worksheet.ListObjects;
// Add a ListObject (table) to the worksheet
int listObjectIndex = listObjects.Add(0, 0, 10, 4, true);
ListObject listObject = listObjects[listObjectIndex];
// Set the name of the ListObject
listObject.DisplayName = "SampleTable";
// Populate the table with some data
worksheet.Cells["A1"].PutValue("Header1");
worksheet.Cells["B1"].PutValue("Header2");
worksheet.Cells["C1"].PutValue("Header3");
worksheet.Cells["D1"].PutValue("Header4");
for (int i = 1; i <= 10; i++)
{
worksheet.Cells[i, 0].PutValue("Row" + i + "Col1");
worksheet.Cells[i, 1].PutValue("Row" + i + "Col2");
worksheet.Cells[i, 2].PutValue("Row" + i + "Col3");
worksheet.Cells[i, 3].PutValue("Row" + i + "Col4");
}
// Update all column names of the tables
listObjects.UpdateColumnName();
// Save the workbook
workbook.Save("ListObjectCollectionExample.xlsx");
return;
}
}
}
```
### See Also
* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ListObject](../listobject/)
* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)
