##WebExtensionReference.StoreType
WebExtensionReference property. Gets and sets the type of marketplace that the store attribute identifies
## WebExtensionReference.StoreType property
Gets and sets the type of marketplace that the store attribute identifies.
```csharp
public WebExtensionStoreType StoreType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;
namespace AsposeCellsExamples
{
public class WebExtensionReferencePropertyStoreTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
int index = webExtensions.Add();
WebExtension webExt = webExtensions[index];
webExt.Reference.Version = "1.0.6.28";
webExt.Reference.StoreName = @"\\server\path\to\addin\";
webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
webExt.Properties.Add("Office.AutoShowTaskpaneWithDocument", "true");
WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
int taskPaneIndex = taskPanes.Add();
WebExtensionTaskPane taskPane = taskPanes[taskPaneIndex];
taskPane.WebExtension = webExt;
taskPane.DockState = "right";
taskPane.IsVisible = true;
taskPane.Width = 350;
workbook.Save("WebExtensionStoreTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [WebExtensionStoreType](../../webextensionstoretype/)
* class [WebExtensionReference](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)
