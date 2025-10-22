##WebExtension.Reference
WebExtension property. Get the primary reference to an Office Addin
## WebExtension.Reference property
Get the primary reference to an Office Add-in.
```csharp
public WebExtensionReference Reference { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;
namespace AsposeCellsExamples
{
public class WebExtensionPropertyReferenceDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a web extension
WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
int webExtIndex = webExtensions.Add();
WebExtension webExt = webExtensions[webExtIndex];
// Set reference properties
webExt.Reference.Version = "1.0.6.28";
webExt.Reference.StoreName = @"\\wanlink.us\DFSRoot\APPS\meZocliq\UAT\Excel_Addin\";
webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
// Add extension properties
webExt.Properties.Add("Office.AutoShowTaskpaneWithDocument", "true");
// Add task pane
WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
int taskPaneIndex = taskPanes.Add();
WebExtensionTaskPane taskPane = taskPanes[taskPaneIndex];
// Configure task pane
taskPane.WebExtension = webExt;
taskPane.DockState = "right";
taskPane.IsVisible = true;
taskPane.Width = 350;
taskPane.Row = 7;
// Save the workbook
workbook.Save("WebExtensionDemo.xlsx");
Console.WriteLine("Web extension with reference properties created successfully.");
}
}
}
```
### See Also
* class [WebExtensionReference](../../webextensionreference/)
* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)
