##Class WebExtensionBindingCollection
Aspose.Cells.WebExtensions.WebExtensionBindingCollection class. Represents the list of binding relationships between an Office Addin and the data in the document
## WebExtensionBindingCollection class
Represents the list of binding relationships between an Office Add-in and the data in the document.
```csharp
public class WebExtensionBindingCollection : CollectionBase<WebExtensionBinding>
```
## Constructors
| Name | Description |
| --- | --- |
| [WebExtensionBindingCollection](webextensionbindingcollection/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.webextensions/webextensionbindingcollection/item/) { get; } | Gets web extension binding relationship by the specific index. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
## Methods
| Name | Description |
| --- | --- |
| [Add](../../aspose.cells.webextensions/webextensionbindingcollection/add/)() | Adds an a binding relationship between an Office Add-in and the data in the document. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(WebExtensionBinding) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(WebExtensionBinding, IComparer&lt;WebExtensionBinding&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, WebExtensionBinding, IComparer&lt;WebExtensionBinding&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(WebExtensionBinding) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(WebExtensionBinding[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(WebExtensionBinding[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, WebExtensionBinding[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;WebExtensionBinding&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;WebExtensionBinding&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;WebExtensionBinding&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;WebExtensionBinding&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;WebExtensionBinding&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;WebExtensionBinding&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;WebExtensionBinding&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;WebExtensionBinding&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;WebExtensionBinding&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;WebExtensionBinding&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(WebExtensionBinding) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(WebExtensionBinding, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(WebExtensionBinding, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(WebExtensionBinding) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(WebExtensionBinding, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(WebExtensionBinding, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.WebExtensions;
using System;
public class WebExtensionsClassWebExtensionBindingCollectionDemo
{
public static void Run()
{
// Create a new workbook for demonstration
Workbook workbook = new Workbook();
try
{
// Create an instance of WebExtensionBindingCollection
WebExtensionBindingCollection bindings = new WebExtensionBindingCollection();
// Add a new binding
int index = bindings.Add();
// Access the binding through the indexer
WebExtensionBinding binding = bindings[index];
// Set properties on the binding (assuming these properties exist based on reference examples)
binding.Id = "binding1";
binding.Type = "table";
binding.Appref = "Sheet1!A1:B5";
// Display basic information
Console.WriteLine($"Created binding with ID: {binding.Id}");
Console.WriteLine($"Total bindings in collection: {bindings.Count}");
// Save the workbook
workbook.Save("WebExtensionBindingCollectionDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error working with WebExtensionBindingCollection: {ex.Message}");
}
}
}
}
```
### See Also
* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [WebExtensionBinding](../webextensionbinding/)
* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)
