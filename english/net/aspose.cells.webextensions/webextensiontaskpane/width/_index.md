---
title: WebExtensionTaskPane.Width
second_title: Aspose.Cells for .NET API Reference
description: WebExtensionTaskPane property. Gets and sets the default width value for this taskpane instance
type: docs
url: /net/aspose.cells.webextensions/webextensiontaskpane/width/
---
## WebExtensionTaskPane.Width property

Gets and sets the default width value for this taskpane instance.

```csharp
public double Width { get; set; }
```

### Examples

```csharp
// Called: taskPane.Width = 350;
[Test]
        public void Property_Width()
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

* class [WebExtensionTaskPane](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


