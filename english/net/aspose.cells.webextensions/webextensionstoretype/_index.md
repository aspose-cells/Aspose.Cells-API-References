---
title: Enum WebExtensionStoreType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.WebExtensions.WebExtensionStoreType enum. Represents the store type of web extension
type: docs
url: /net/aspose.cells.webextensions/webextensionstoretype/
---
## WebExtensionStoreType enumeration

Represents the store type of web extension.

```csharp
public enum WebExtensionStoreType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| OMEX | `0` | Specifies that the store type is Office.com. |
| SPCatalog | `1` | Specifies that the store type is SharePoint corporate catalog. |
| SPApp | `2` | Specifies that the store type is a SharePoint web application. |
| Exchange | `3` | Specifies that the store type is an Exchange server. |
| FileSystem | `4` | Specifies that the store type is a file system share. |
| Registry | `5` | Specifies that the store type is the system registry. |
| ExCatalog | `6` | Specifies that the store type is Centralized Deployment via Exchange. |

### Examples

```csharp
// Called: webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
[Test]
        public void Type_WebExtensionStoreType()
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
            workbook.Save(Constants.destPath + "Test_002.xlsx");
            workbook = new Workbook(Constants.destPath + "Test_002.xlsx");
            Assert.AreEqual(1, workbook.Worksheets.WebExtensions.Count);
            Assert.AreEqual(1, workbook.Worksheets.WebExtensionTaskPanes.Count);
        }
```

### See Also

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


