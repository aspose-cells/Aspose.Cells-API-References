##Class WebExtensionReferenceCollection
Aspose.Cells.WebExtensions.WebExtensionReferenceCollection class. Represents the list of web extension reference
## WebExtensionReferenceCollection class
Represents the list of web extension reference.
```csharp
public class WebExtensionReferenceCollection : CollectionBase<WebExtensionReference>
```
## Constructors
| Name | Description |
| --- | --- |
| [WebExtensionReferenceCollection](webextensionreferencecollection/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.webextensions/webextensionreferencecollection/item/) { get; } | Gets web extension by the specific index. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
## Methods
| Name | Description |
| --- | --- |
| [Add](../../aspose.cells.webextensions/webextensionreferencecollection/add/)() | Adds an empty reference of web extension. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(WebExtensionReference) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(WebExtensionReference, IComparer&lt;WebExtensionReference&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, WebExtensionReference, IComparer&lt;WebExtensionReference&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(WebExtensionReference) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(WebExtensionReference[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(WebExtensionReference[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, WebExtensionReference[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;WebExtensionReference&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;WebExtensionReference&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;WebExtensionReference&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;WebExtensionReference&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;WebExtensionReference&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;WebExtensionReference&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;WebExtensionReference&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;WebExtensionReference&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;WebExtensionReference&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;WebExtensionReference&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(WebExtensionReference) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(WebExtensionReference, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(WebExtensionReference, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(WebExtensionReference) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(WebExtensionReference, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(WebExtensionReference, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells.WebExtensions;
using System;
public class WebExtensionsClassWebExtensionReferenceCollectionDemo
{
public static void Run()
{
try
{
// Create an instance of WebExtensionReferenceCollection
WebExtensionReferenceCollection references = new WebExtensionReferenceCollection();
// Add a new web extension reference
int index = references.Add();
// Access the added reference (read-only property)
WebExtensionReference reference = references[index];
Console.WriteLine($"Added web extension reference at index: {index}");
Console.WriteLine($"Total references count: {references.Count}");
}
catch (Exception ex)
{
Console.WriteLine($"Error working with WebExtensionReferenceCollection: {ex.Message}");
}
}
}
}
```
### See Also
* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [WebExtensionReference](../webextensionreference/)
* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)
