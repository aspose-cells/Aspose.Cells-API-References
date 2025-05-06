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
// Called: webExt.Reference.StoreType = WebExtensionStoreType.OMEX;
[Test]
        public void Type_WebExtensionStoreType()
        {
            Workbook workbook = new Workbook();
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int index = webExtensions.Add();
            WebExtension webExt = webExtensions[index];
            //version=&quot;1.0.6.28&quot; store=&quot;\\wanlink.us\DFSRoot\APPS\meZocliq\UAT\Excel_Addin\&quot; storeType=&quot;Filesystem&quot;
            webExt.Reference.Id = &quot;wa104104476&quot;;
            webExt.Reference.Version = &quot;1.3.0.0&quot;;
            webExt.Reference.StoreName = @&quot;en-US&quot;;
            webExt.Reference.StoreType = WebExtensionStoreType.OMEX;
            webExt.Properties.Add(&quot;sku&quot;, &quot;\&quot;peoplebar-giant\&quot;&quot;);
            webExt.Properties.Add(&quot;theme&quot;, &quot;\&quot;giant-redwhiteblack\&quot;&quot;);
            webExt.Properties.Add(&quot;shape&quot;, &quot;\&quot;muscle-people\&quot;&quot;);
            webExt.Properties.Add(&quot;layout-element-title&quot;, &quot;\&quot;NUMBERS ABOUT THE APP\&quot;&quot;);
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            shapes.AddShape(MsoDrawingType.WebExtension, 0, 0, 0, 0, 500, 500);
            WebExtensionShape wShape = (WebExtensionShape)shapes[0];
            wShape.WebExtension = webExt;


            //      workbook.Worksheets.Add();
            workbook.Save(Constants.destPath + &quot;CELLSNET46124.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSNET46124.xlsx&quot;);
        }
```

### See Also

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


