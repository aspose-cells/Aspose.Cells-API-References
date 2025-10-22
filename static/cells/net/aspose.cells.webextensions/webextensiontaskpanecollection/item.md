##WebExtensionTaskPaneCollection.Item
WebExtensionTaskPaneCollection property. Gets task pane by the specific index
## WebExtensionTaskPaneCollection indexer
Gets task pane by the specific index.
```csharp
public WebExtensionTaskPane this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The index. |
### Return Value
The task pane.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;
namespace AsposeCellsExamples
{
public class WebExtensionTaskPaneCollectionPropertyItemDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
int extensionIndex = webExtensions.Add();
WebExtension webExt = webExtensions[extensionIndex];
webExt.Reference.Version = "1.0.0";
webExt.Reference.StoreName = @"C:\\Extensions\\";
webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
webExt.Properties.Add("Office.AutoShowTaskpane", "true");
WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
int paneIndex = taskPanes.Add();
WebExtensionTaskPane taskPane = taskPanes[paneIndex];
taskPane.WebExtension = webExt;
taskPane.DockState = "right";
taskPane.IsVisible = true;
taskPane.Width = 300;
// Demonstrate Item property usage
WebExtensionTaskPane retrievedPane = taskPanes[paneIndex];
Console.WriteLine($"Retrieved task pane width: {retrievedPane.Width}");
workbook.Save("WebExtensionDemo.xlsx");
}
}
}
```
### See Also
* class [WebExtensionTaskPane](../../webextensiontaskpane/)
* class [WebExtensionTaskPaneCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)
