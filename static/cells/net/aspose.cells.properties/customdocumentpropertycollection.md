##Class CustomDocumentPropertyCollection
Aspose.Cells.Properties.CustomDocumentPropertyCollection class. A collection of custom document properties
## CustomDocumentPropertyCollection class
A collection of custom document properties.
```csharp
public class CustomDocumentPropertyCollection : DocumentPropertyCollection
```
## Properties
| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.properties/documentpropertycollection/item/) { get; } | Returns a [`DocumentProperty`](../documentproperty/) object by index.(Inherited from [`DocumentPropertyCollection`](../documentpropertycollection/).) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| virtual [Item](../../aspose.cells.properties/documentpropertycollection/item/) { get; } | Returns a [`DocumentProperty`](../documentproperty/) object by the name of the property.(Inherited from [`DocumentPropertyCollection`](../documentpropertycollection/).) |
## Methods
| Name | Description |
| --- | --- |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add/#add)(string, bool) | Creates a new custom document property of the **PropertyType.Boolean** data type. |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add/#add_3)(string, DateTime) | Creates a new custom document property of the **PropertyType.DateTime** data type. |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add/#add_1)(string, double) | Creates a new custom document property of the **PropertyType.Float** data type. |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add/#add_2)(string, int) | Creates a new custom document property of the **PropertyType.Number** data type. |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add/#add_4)(string, string) | Creates a new custom document property of the **PropertyType.String** data type. |
| [AddLinkToContent](../../aspose.cells.properties/customdocumentpropertycollection/addlinktocontent/)(string, string) | Creates a new custom document property which links to content. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(DocumentProperty) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(DocumentProperty, IComparer&lt;DocumentProperty&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, DocumentProperty, IComparer&lt;DocumentProperty&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(DocumentProperty) |  |
| [Contains](../../aspose.cells.properties/documentpropertycollection/contains/)(string) | Returns true if a property with the specified name exists in the collection.(Inherited from [`DocumentPropertyCollection`](../documentpropertycollection/).) |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(DocumentProperty[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(DocumentProperty[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, DocumentProperty[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;DocumentProperty&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;DocumentProperty&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;DocumentProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;DocumentProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;DocumentProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;DocumentProperty&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;DocumentProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;DocumentProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;DocumentProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;DocumentProperty&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DocumentProperty) |  |
| [IndexOf](../../aspose.cells.properties/documentpropertycollection/indexof/)(string) | Gets the index of a property by name.(Inherited from [`DocumentPropertyCollection`](../documentpropertycollection/).) |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DocumentProperty, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DocumentProperty, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DocumentProperty) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DocumentProperty, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DocumentProperty, int, int) |  |
| [Remove](../../aspose.cells.properties/documentpropertycollection/remove/)(string) | Removes a property with the specified name from the collection.(Inherited from [`DocumentPropertyCollection`](../documentpropertycollection/).) |
| [RemoveAt](../../aspose.cells.properties/documentpropertycollection/removeat/)(int) | Removes a property at the specified index. (2 methods) |
| [UpdateLinkedPropertyValue](../../aspose.cells.properties/customdocumentpropertycollection/updatelinkedpropertyvalue/)() | Updates values of all custom properties that are linked to content(use cell value of linked range to update value of custom property). |
| [UpdateLinkedRange](../../aspose.cells.properties/customdocumentpropertycollection/updatelinkedrange/)() | Updates all ranges that are linked to custom properties(use the value of custom document property to update cell value of linked range). |
### Remarks
Each [`DocumentProperty`](../documentproperty/) object represents a custom property of a container document.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Properties;
using System;
public class CustomDocumentPropertyCollectionDemo
{
public static void CustomDocumentPropertyCollectionExample()
{
// Instantiate a Workbook object
Workbook workbook = new Workbook();
// Retrieve a list of all custom document properties of the Excel file
CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
// Add custom document properties
customProperties.Add("Author", "John Doe");
customProperties.Add("Revision", 3);
customProperties.Add("LastModified", DateTime.Now);
customProperties.Add("IsFinal", true);
customProperties.Add("Rating", 4.5);
// Add a linked custom document property
customProperties.AddLinkToContent("LinkedProperty", "Sheet1!A1");
// Update linked property values
//customProperties.UpdateLinkedPropertyValue();
customProperties.UpdateLinkedRange();
// Accessing custom document properties
DocumentProperty authorProperty = customProperties["Author"];
DocumentProperty revisionProperty = customProperties["Revision"];
DocumentProperty lastModifiedProperty = customProperties["LastModified"];
DocumentProperty isFinalProperty = customProperties["IsFinal"];
DocumentProperty ratingProperty = customProperties["Rating"];
DocumentProperty linkedProperty = customProperties["LinkedProperty"];
// Print custom document properties
Console.WriteLine($"Author: {authorProperty.Value}");
Console.WriteLine($"Revision: {revisionProperty.ToInt()}");
Console.WriteLine($"Last Modified: {lastModifiedProperty.ToDateTime()}");
Console.WriteLine($"Is Final: {isFinalProperty.ToBool()}");
Console.WriteLine($"Rating: {ratingProperty.ToDouble()}");
Console.WriteLine($"Linked Property: {linkedProperty.Value}");
// Save the workbook
workbook.Save("CustomDocumentPropertiesExample.xlsx");
workbook.Save("CustomDocumentPropertiesExample.pdf");
}
}
}
```
### See Also
* class [DocumentPropertyCollection](../documentpropertycollection/)
* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)
