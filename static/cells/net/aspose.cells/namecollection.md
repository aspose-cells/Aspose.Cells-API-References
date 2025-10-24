##Class NameCollection
Aspose.Cells.NameCollection class. Represents a collection of all the Name objects in the spreadsheet
## NameCollection class
Represents a collection of all the [`Name`](../name/) objects in the spreadsheet.
```csharp
public class NameCollection : CollectionBase<Name>
```
## Properties
| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/namecollection/item/) { get; } | Gets the [`Name`](../name/) element at the specified index. (2 indexers) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
## Methods
| Name | Description |
| --- | --- |
| [Add](../../aspose.cells/namecollection/add/)(string) | Defines a new name. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Name) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Name, IComparer&lt;Name&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Name, IComparer&lt;Name&gt;) |  |
| [Clear](../../aspose.cells/namecollection/clear/#clear)() | Remove all defined names which are not referenced by the formulas and data source. If the defined name is referred, we only set Name.ReferTo as null and hide them. (2 methods) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Name) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Name[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Name[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Name[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Name&gt;) |  |
| [Filter](../../aspose.cells/namecollection/filter/)(NameScopeType, int) | Gets all defined name by scope. |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Name&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Name&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Name&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Name&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Name&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Name&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Name&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Name&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Name&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Name) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Name, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Name, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Name) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Name, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Name, int, int) |  |
| [Remove](../../aspose.cells/namecollection/remove/#remove)(string) | Remove the name. |
| [Remove](../../aspose.cells/namecollection/remove/#remove_1)(string[]) | Remove an array of name |
| [RemoveAt](../../aspose.cells/namecollection/removeat/#removeat)(int) | Remove the name at the specific index. (2 methods) |
| [RemoveDuplicateNames](../../aspose.cells/namecollection/removeduplicatenames/)() | Remove the duplicate defined names |
| [Sort](../../aspose.cells/namecollection/sort/)() | Sorts defined names. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class NameCollectionDemo
{
public static void NameCollectionExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the worksheet collection
WorksheetCollection worksheets = workbook.Worksheets;
// Access the name collection
NameCollection names = worksheets.Names;
// Add a new name to the collection
int nameIndex = names.Add("MyNamedRange");
Name name = names[nameIndex];
// Set the refers to property for the name
name.RefersTo = "=Sheet1!$A$1:$A$10";
// Access and modify properties of the name
name.Comment = "This is a named range for demonstration.";
name.IsVisible = true;
// Add another name
int anotherNameIndex = names.Add("AnotherNamedRange");
Name anotherName = names[anotherNameIndex];
anotherName.RefersTo = "=Sheet1!$B$1:$B$10";
// Remove a name by text
names.Remove("AnotherNamedRange");
// Remove a name by index
names.RemoveAt(nameIndex);
// Clear all names
names.Clear();
// Save the workbook
workbook.Save("NameCollectionExample.xlsx");
return;
}
}
}
```
### See Also
* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Name](../name/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
