---
title: Class WebExtensionTaskPane
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.WebExtensions.WebExtensionTaskPane class. Represents a persisted taskpane object
type: docs
url: /net/aspose.cells.webextensions/webextensiontaskpane/
---
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
// Called: WebExtensionTaskPane taskPane = taskPanes[index1];
public void WebExtensions_Type_WebExtensionTaskPane()
{
    Workbook workbook = new Workbook();
    WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
    int index = webExtensions.Add();
    WebExtension webExt = webExtensions[index];
    //version="1.0.6.28" store="\\wanlink.us\DFSRoot\APPS\meZocliq\UAT\Excel_Addin\" storeType="Filesystem"
    webExt.Reference.Version = "1.0.6.28";
    webExt.Reference.StoreName = @"\\wanlink.us\DFSRoot\APPS\meZocliq\UAT\Excel_Addin\";
    webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
    webExt.Properties.Add("Office.AutoShowTaskpaneWithDocument", "true");

    WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
    int index1 = taskPanes.Add();
    WebExtensionTaskPane taskPane = taskPanes[index1];

    taskPane.WebExtension = webExt;
    taskPane.DockState = "right";
    taskPane.IsVisible = true;
    taskPane.Width = 350;
    taskPane.Row = 7;
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    Assert.AreEqual(1, workbook.Worksheets.WebExtensions.Count);
    Assert.AreEqual(1, workbook.Worksheets.WebExtensionTaskPanes.Count);
}
```

### See Also

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


