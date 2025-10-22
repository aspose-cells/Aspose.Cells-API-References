##WebExtensionReference.StoreName
WebExtensionReference property. Gets and sets the instance of the marketplace where the Office Addin is stored.
## WebExtensionReference.StoreName property
Gets and sets the instance of the marketplace where the Office Add-in is stored. .
```csharp
public string StoreName { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;
namespace AsposeCellsExamples
{
public class WebExtensionReferencePropertyStoreNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a web extension
WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
int extensionIndex = webExtensions.Add();
WebExtension webExt = webExtensions[extensionIndex];
// Set web extension reference properties including StoreName
webExt.Reference.Version = "1.0.6.28";
webExt.Reference.StoreName = @"\\wanlink.us\DFSRoot\APPS\meZocliq\UAT\Excel_Addin\";
webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
webExt.Properties.Add("Office.AutoShowTaskpaneWithDocument", "true");
// Add a task pane for the web extension
WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
int paneIndex = taskPanes.Add();
WebExtensionTaskPane taskPane = taskPanes[paneIndex];
taskPane.WebExtension = webExt;
taskPane.DockState = "right";
taskPane.IsVisible = true;
taskPane.Width = 350;
// Save the workbook
workbook.Save("WebExtensionDemo.xlsx");
Console.WriteLine("Workbook with web extension saved successfully.");
}
}
}
```
### See Also
* class [WebExtensionReference](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)
