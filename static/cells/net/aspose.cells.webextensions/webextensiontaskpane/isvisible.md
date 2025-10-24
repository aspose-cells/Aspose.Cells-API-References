##WebExtensionTaskPane.IsVisible
WebExtensionTaskPane property. Indicates whether the Task Pane shows as visible by default when the document opens
## WebExtensionTaskPane.IsVisible property
Indicates whether the Task Pane shows as visible by default when the document opens.
```csharp
public bool IsVisible { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;
namespace AsposeCellsExamples
{
public class WebExtensionTaskPanePropertyIsVisibleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a web extension
WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
int extensionIndex = webExtensions.Add();
WebExtension webExt = webExtensions[extensionIndex];
// Configure web extension properties
webExt.Reference.Version = "1.0.0";
webExt.Reference.StoreName = @"C:\\Extensions\\";
webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
// Add a task pane
WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
int paneIndex = taskPanes.Add();
WebExtensionTaskPane taskPane = taskPanes[paneIndex];
// Configure task pane properties
taskPane.WebExtension = webExt;
taskPane.DockState = "right";
taskPane.Width = 300;
// Demonstrate IsVisible property
Console.WriteLine("Initial IsVisible: " + taskPane.IsVisible);
taskPane.IsVisible = true;
Console.WriteLine("After setting to true: " + taskPane.IsVisible);
// Save the workbook
workbook.Save("WebExtensionTaskPaneDemo.xlsx");
}
}
}
```
### See Also
* class [WebExtensionTaskPane](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)
