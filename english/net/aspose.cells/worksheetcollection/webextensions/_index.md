---
title: WorksheetCollection.WebExtensions
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection property. Gets the list of task panes
type: docs
url: /net/aspose.cells/worksheetcollection/webextensions/
---
## WorksheetCollection.WebExtensions property

Gets the list of task panes.

```csharp
public WebExtensionCollection WebExtensions { get; }
```

### Examples

```csharp
// Called: WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
[Test]
        public void Property_WebExtensions()
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

* class [WebExtensionCollection](../../../aspose.cells.webextensions/webextensioncollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


