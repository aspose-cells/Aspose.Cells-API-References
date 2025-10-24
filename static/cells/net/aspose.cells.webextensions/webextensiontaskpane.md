##Class WebExtensionTaskPane
Aspose.Cells.WebExtensions.WebExtensionTaskPane class. Represents a persisted taskpane object
## WebExtensionTaskPane class
Represents a persisted taskpane object.
```csharp
public class WebExtensionTaskPane
```
## Properties
| Name | Description |
| --- | --- |
| [DockState](../../aspose.cells.webextensions/webextensiontaskpane/dockstate/) { get; set; } | Gets and sets the last-docked location of this taskpane object. |
| [IsLocked](../../aspose.cells.webextensions/webextensiontaskpane/islocked/) { get; set; } | Indicates whether the taskpane is locked to the document in the UI and cannot be closed by the user. |
| [IsVisible](../../aspose.cells.webextensions/webextensiontaskpane/isvisible/) { get; set; } | Indicates whether the Task Pane shows as visible by default when the document opens. |
| [Row](../../aspose.cells.webextensions/webextensiontaskpane/row/) { get; set; } | Gets and sets the index, enumerating from the outside to the inside, of this taskpane among other persisted taskpanes docked in the same default location. |
| [WebExtension](../../aspose.cells.webextensions/webextensiontaskpane/webextension/) { get; set; } | Gets and sets the web extension part associated with the taskpane instance |
| [Width](../../aspose.cells.webextensions/webextensiontaskpane/width/) { get; set; } | Gets and sets the default width value for this taskpane instance. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;
namespace AsposeCellsExamples
{
public class WebExtensionsClassWebExtensionTaskPaneDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
int webExtIndex = webExtensions.Add();
WebExtension webExt = webExtensions[webExtIndex];
webExt.Reference.Version = "1.0.6.28";
webExt.Reference.StoreName = @"\\wanlink.us\DFSRoot\APPS\meZocliq\UAT\Excel_Addin\";
webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
webExt.Properties.Add("Office.AutoShowTaskpaneWithDocument", "true");
WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
int taskPaneIndex = taskPanes.Add();
WebExtensionTaskPane taskPane = taskPanes[taskPaneIndex];
taskPane.WebExtension = webExt;
taskPane.DockState = "right";
taskPane.IsVisible = true;
taskPane.Width = 350;
taskPane.Row = 7;
workbook.Save("WebExtensionTaskPaneDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)
