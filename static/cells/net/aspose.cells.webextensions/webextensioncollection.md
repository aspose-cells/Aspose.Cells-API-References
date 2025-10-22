##Class WebExtensionCollection
Aspose.Cells.WebExtensions.WebExtensionCollection class. Represents the list of web extension
## WebExtensionCollection class
Represents the list of web extension.
```csharp
public class WebExtensionCollection : CollectionBase<WebExtension>
```
## Properties
| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.webextensions/webextensioncollection/item/) { get; } | Gets web extension by the specific index. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
## Methods
| Name | Description |
| --- | --- |
| [Add](../../aspose.cells.webextensions/webextensioncollection/add/)() | Adds a web extension. |
| [AddWebVideoPlayer](../../aspose.cells.webextensions/webextensioncollection/addwebvideoplayer/)(string, bool, int, int) | Add a web video player into exel. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(WebExtension) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(WebExtension, IComparer&lt;WebExtension&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, WebExtension, IComparer&lt;WebExtension&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(WebExtension) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(WebExtension[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(WebExtension[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, WebExtension[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;WebExtension&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;WebExtension&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;WebExtension&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;WebExtension&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;WebExtension&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;WebExtension&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;WebExtension&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;WebExtension&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;WebExtension&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;WebExtension&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(WebExtension) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(WebExtension, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(WebExtension, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(WebExtension) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(WebExtension, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(WebExtension, int, int) |  |
| [RemoveAt](../../aspose.cells.webextensions/webextensioncollection/removeat/#removeat)(int) | Remove web extension by the index. (2 methods) |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class WebExtensionsClassWebExtensionCollectionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the WebExtensionCollection
WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
// Add a new web extension
int index = webExtensions.Add();
WebExtension webExt = webExtensions[index];
// Set web extension properties
webExt.Reference.Id = "wa104104476";
webExt.Reference.Version = "1.3.0.0";
webExt.Reference.StoreName = "en-US";
webExt.Reference.StoreType = WebExtensionStoreType.OMEX;
// Add custom properties
webExt.Properties.Add("sku", "peoplebar-giant");
webExt.Properties.Add("theme", "giant-redwhiteblack");
webExt.Properties.Add("shape", "muscle-people");
webExt.Properties.Add("layout-element-title", "NUMBERS ABOUT THE APP");
// Create a shape to host the web extension
ShapeCollection shapes = workbook.Worksheets[0].Shapes;
shapes.AddShape(MsoDrawingType.WebExtension, 0, 0, 0, 0, 500, 500);
WebExtensionShape wShape = (WebExtensionShape)shapes[0];
wShape.WebExtension = webExt;
// Save the workbook
workbook.Save("web_extension_demo.xlsx");
}
}
}
```
### See Also
* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [WebExtension](../webextension/)
* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)
