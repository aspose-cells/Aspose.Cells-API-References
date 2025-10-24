##WorksheetCollection.WebExtensionTaskPanes
WorksheetCollection property. Gets the list of task panes
## WorksheetCollection.WebExtensionTaskPanes property
Gets the list of task panes.
```csharp
public WebExtensionTaskPaneCollection WebExtensionTaskPanes { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;
namespace AsposeCellsExamples
{
public class WorksheetCollectionPropertyWebExtensionTaskPanesDemo
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
webExt.Reference.Version = "1.0.6.28";
webExt.Reference.StoreName = @"\\wanlink.us\DFSRoot\APPS\meZocliq\UAT\Excel_Addin\";
webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
webExt.Properties.Add("Office.AutoShowTaskpaneWithDocument", "true");
// Add and configure task pane
WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
int taskPaneIndex = taskPanes.Add();
WebExtensionTaskPane taskPane = taskPanes[taskPaneIndex];
taskPane.WebExtension = webExt;
taskPane.DockState = "right";
taskPane.IsVisible = true;
taskPane.Width = 350;
taskPane.Row = 7;
// Save the workbook
workbook.Save("WebExtensionTaskPaneDemo.xlsx");
Console.WriteLine("Workbook with web extension task pane created successfully.");
}
}
}
```
### See Also
* class [WebExtensionTaskPaneCollection](../../../aspose.cells.webextensions/webextensiontaskpanecollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
