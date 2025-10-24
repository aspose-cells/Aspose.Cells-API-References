##WebExtensionTaskPane.Row
WebExtensionTaskPane property. Gets and sets the index enumerating from the outside to the inside of this taskpane among other persisted taskpanes docked in the same default location
## WebExtensionTaskPane.Row property
Gets and sets the index, enumerating from the outside to the inside, of this taskpane among other persisted taskpanes docked in the same default location.
```csharp
public int Row { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;
namespace AsposeCellsExamples
{
public class WebExtensionTaskPanePropertyRowDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a web extension
WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
int webExtIndex = webExtensions.Add();
WebExtension webExt = webExtensions[webExtIndex];
// Configure web extension properties
webExt.Reference.Version = "1.0.0";
webExt.Reference.StoreName = @"C:\Extensions\";
webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
// Add a task pane
WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
int paneIndex = taskPanes.Add();
WebExtensionTaskPane taskPane = taskPanes[paneIndex];
// Configure task pane properties
taskPane.WebExtension = webExt;
taskPane.DockState = "right";
taskPane.IsVisible = true;
taskPane.Width = 300;
// Demonstrate Row property usage
taskPane.Row = 5; // Set row position
// Save the workbook
workbook.Save("WebExtensionTaskPaneDemo.xlsx");
Console.WriteLine("Workbook saved with web extension task pane (Row: " + taskPane.Row + ")");
}
}
}
```
### See Also
* class [WebExtensionTaskPane](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)
