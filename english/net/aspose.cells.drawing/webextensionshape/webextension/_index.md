---
title: WebExtensionShape.WebExtension
second_title: Aspose.Cells for .NET API Reference
description: WebExtensionShape property. Gets and set the web extension
type: docs
url: /net/aspose.cells.drawing/webextensionshape/webextension/
---
## WebExtensionShape.WebExtension property

Gets and set the web extension.

```csharp
public WebExtension WebExtension { get; set; }
```

### Examples

```csharp
// Called: wShape.WebExtension = webExt;
public void WebExtensionShape_Property_WebExtension()
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
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [WebExtension](../../../aspose.cells.webextensions/webextension/)
* class [WebExtensionShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


