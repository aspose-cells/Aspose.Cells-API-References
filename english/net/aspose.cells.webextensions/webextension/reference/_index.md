---
title: WebExtension.Reference
second_title: Aspose.Cells for .NET API Reference
description: WebExtension property. Get the primary reference to an Office Addin
type: docs
url: /net/aspose.cells.webextensions/webextension/reference/
---
## WebExtension.Reference property

Get the primary reference to an Office Add-in.

```csharp
public WebExtensionReference Reference { get; }
```

### Examples

```csharp
// Called: webExt.Reference.StoreName = @"\\wanlink.us\DFSRoot\APPS\meZocliq\UAT\Excel_Addin\";
public void WebExtension_Property_Reference()
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

* class [WebExtensionReference](../../webextensionreference/)
* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


