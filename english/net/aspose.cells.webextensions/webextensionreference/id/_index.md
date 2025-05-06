---
title: WebExtensionReference.Id
second_title: Aspose.Cells for .NET API Reference
description: WebExtensionReference property. Gets and sets the identifier associated with the Office Addin within a catalog provider. The identifier MUST be unique within a catalog provider
type: docs
url: /net/aspose.cells.webextensions/webextensionreference/id/
---
## WebExtensionReference.Id property

Gets and sets the identifier associated with the Office Add-in within a catalog provider. The identifier MUST be unique within a catalog provider.

```csharp
public string Id { get; set; }
```

### Examples

```csharp
// Called: webExt.Reference.Id = &amp;quot;wa104104476&amp;quot;;
[Test]
        public void Property_Id()
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

* class [WebExtensionReference](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


