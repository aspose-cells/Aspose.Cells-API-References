---
title: WebExtensionCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: WebExtensionCollection property. Gets web extension by the specific index
type: docs
url: /net/aspose.cells.webextensions/webextensioncollection/item/
---
## WebExtensionCollection indexer

Gets web extension by the specific index.

```csharp
public WebExtension this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index. |

### Return Value

The web extension.

### Examples

```csharp
// Called: WebExtension webExt = webExtensions[index];
[Test]
        public void Property_Int32_()
        {
            Workbook workbook = new Workbook();
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int index = webExtensions.AddWebVideoPlayer(&quot;https://www.youtube.com/watch?v=z0hFbzPPfm8&quot;, true, 0, 0);
            WebExtension webExt = webExtensions[index];
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            shapes.AddShape(MsoDrawingType.WebExtension, 0, 0, 0, 0, 410, 730);
            WebExtensionShape wShape = (WebExtensionShape)shapes[0];
            wShape.WebExtension = webExt;
            workbook.Save(Constants.destPath + &quot;InsertYoutubeToExcel.xlsx&quot;);
        }
```

### See Also

* class [WebExtension](../../webextension/)
* class [WebExtensionCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


