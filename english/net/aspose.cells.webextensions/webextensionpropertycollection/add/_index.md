---
title: WebExtensionPropertyCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: WebExtensionPropertyCollection method. Adds web extension property
type: docs
url: /net/aspose.cells.webextensions/webextensionpropertycollection/add/
---
## WebExtensionPropertyCollection.Add method

Adds web extension property.

```csharp
public int Add(string name, string value)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of property. |
| value | String | The value of property. |

### Return Value

The index of added property.

### Examples

```csharp
// Called: webExt.Properties.Add("sku", "\"peoplebar-giant\"");
public void WebExtensionPropertyCollection_Method_Add()
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

* class [WebExtensionPropertyCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


