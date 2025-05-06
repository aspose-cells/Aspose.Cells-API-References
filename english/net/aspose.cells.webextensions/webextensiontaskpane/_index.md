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
[Test]
        public void Type_WebExtensionTaskPane()
        {
            Workbook workbook = new Workbook();
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int index = webExtensions.Add();
            WebExtension webExt = webExtensions[index];
            //version=&quot;1.0.6.28&quot; store=&quot;\\wanlink.us\DFSRoot\APPS\meZocliq\UAT\Excel_Addin\&quot; storeType=&quot;Filesystem&quot;
            webExt.Reference.Version = &quot;1.0.6.28&quot;;
            webExt.Reference.StoreName = @&quot;\\wanlink.us\DFSRoot\APPS\meZocliq\UAT\Excel_Addin\&quot;;
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            webExt.Properties.Add(&quot;Office.AutoShowTaskpaneWithDocument&quot;, &quot;true&quot;);

            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int index1 = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[index1];

            taskPane.WebExtension = webExt;
            taskPane.DockState = &quot;right&quot;;
            taskPane.IsVisible = true;
            taskPane.Width = 350;
            taskPane.Row = 7;
            workbook.Save(Constants.destPath + &quot;Test_002.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;Test_002.xlsx&quot;);
            Assert.AreEqual(1, workbook.Worksheets.WebExtensions.Count);
            Assert.AreEqual(1, workbook.Worksheets.WebExtensionTaskPanes.Count);
        }
```

### See Also

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


