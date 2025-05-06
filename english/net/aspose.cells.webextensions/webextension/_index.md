---
title: Class WebExtension
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.WebExtensions.WebExtension class. Represents an Office Addin instance
type: docs
url: /net/aspose.cells.webextensions/webextension/
---
## WebExtension class

Represents an Office Add-in instance.

```csharp
public class WebExtension
```

## Properties

| Name | Description |
| --- | --- |
| [AlterReferences](../../aspose.cells.webextensions/webextension/alterreferences/) { get; } | Gets a list of alter references. |
| [Bindings](../../aspose.cells.webextensions/webextension/bindings/) { get; } | Gets all bindings relationship between an Office Add-in and the data in the document. |
| [Id](../../aspose.cells.webextensions/webextension/id/) { get; set; } | Gets and sets the uniquely identifies the Office Add-in instance in the current document. |
| [IsFrozen](../../aspose.cells.webextensions/webextension/isfrozen/) { get; set; } | Indicates whether the user can interact with the Office Add-in or not. |
| [Properties](../../aspose.cells.webextensions/webextension/properties/) { get; } | Gets all properties of web extension. |
| [Reference](../../aspose.cells.webextensions/webextension/reference/) { get; } | Get the primary reference to an Office Add-in. |

### Examples

```csharp
// Called: WebExtension webExt = webExtensions[index];
[Test]
        public void Type_WebExtension()
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


