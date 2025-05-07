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
// Called: webExt.Reference.Id = "wa104104476";
[Test]
        public void Property_Id()
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

* class [WebExtensionReference](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


