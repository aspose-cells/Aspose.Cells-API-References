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
// Called: webExt.Reference.StoreName = @"en-US";
[Test]
        public void Property_Reference()
        {
            Workbook workbook = new Workbook();
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int index = webExtensions.Add();
            WebExtension webExt = webExtensions[index];
            //version="1.0.6.28" store="\\wanlink.us\DFSRoot\APPS\meZocliq\UAT\Excel_Addin\" storeType="Filesystem"
            webExt.Reference.Id = "wa104104476";
            webExt.Reference.Version = "1.3.0.0";
            webExt.Reference.StoreName = @"en-US";
            webExt.Reference.StoreType = WebExtensionStoreType.OMEX;
            webExt.Properties.Add("sku", "\"peoplebar-giant\"");
            webExt.Properties.Add("theme", "\"giant-redwhiteblack\"");
            webExt.Properties.Add("shape", "\"muscle-people\"");
            webExt.Properties.Add("layout-element-title", "\"NUMBERS ABOUT THE APP\"");
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            shapes.AddShape(MsoDrawingType.WebExtension, 0, 0, 0, 0, 500, 500);
            WebExtensionShape wShape = (WebExtensionShape)shapes[0];
            wShape.WebExtension = webExt;


            //      workbook.Worksheets.Add();
            workbook.Save(Constants.destPath + "CELLSNET46124.xlsx");
            workbook = new Workbook(Constants.destPath + "CELLSNET46124.xlsx");
        }
```

### See Also

* class [WebExtensionReference](../../webextensionreference/)
* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


