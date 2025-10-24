##Class ContentTypePropertyCollection
Aspose.Cells.Properties.ContentTypePropertyCollection class. A collection of ContentTypeProperty objects that represent additional information
## ContentTypePropertyCollection class
A collection of [`ContentTypeProperty`](../contenttypeproperty/) objects that represent additional information.
```csharp
public class ContentTypePropertyCollection : CollectionBase<ContentTypeProperty>
```
## Properties
| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.properties/contenttypepropertycollection/item/) { get; } | Gets the content type property by the specific index. (2 indexers) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
## Methods
| Name | Description |
| --- | --- |
| [Add](../../aspose.cells.properties/contenttypepropertycollection/add/#add)(string, string) | Adds content type property information. |
| [Add](../../aspose.cells.properties/contenttypepropertycollection/add/#add_1)(string, string, string) | Adds content type property information. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ContentTypeProperty) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ContentTypeProperty, IComparer&lt;ContentTypeProperty&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ContentTypeProperty, IComparer&lt;ContentTypeProperty&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ContentTypeProperty) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ContentTypeProperty[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ContentTypeProperty[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ContentTypeProperty[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ContentTypeProperty&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ContentTypeProperty&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ContentTypeProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ContentTypeProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ContentTypeProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ContentTypeProperty&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ContentTypeProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ContentTypeProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ContentTypeProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ContentTypeProperty&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ContentTypeProperty) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ContentTypeProperty, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ContentTypeProperty, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ContentTypeProperty) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ContentTypeProperty, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ContentTypeProperty, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Properties;
using System;
public class ContentTypePropertyCollectionDemo
{
public static void ContentTypePropertyCollectionExample()
{
// Instantiating a Workbook object
Workbook workbook = new Workbook();
// Add a new property to the ContentTypePropertyCollection
workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");
// Accessing the ContentTypePropertyCollection
ContentTypePropertyCollection contentTypeProperties = workbook.ContentTypeProperties;
// Displaying the count of properties
Console.WriteLine("Number of ContentTypeProperties: " + contentTypeProperties.Count);
// Accessing a specific property by index
ContentTypeProperty property = contentTypeProperties[0];
Console.WriteLine("Property Name: " + property.Name);
Console.WriteLine("Property Value: " + property.Value);
Console.WriteLine("Property Type: " + property.Type);
// Modifying the capacity of the collection
contentTypeProperties.Capacity = 10;
Console.WriteLine("New Capacity: " + contentTypeProperties.Capacity);
// Save the Excel file
workbook.Save("ContentTypePropertyCollectionExample.xlsx");
workbook.Save("ContentTypePropertyCollectionExample.pdf");
}
}
}
```
### See Also
* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ContentTypeProperty](../contenttypeproperty/)
* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)
