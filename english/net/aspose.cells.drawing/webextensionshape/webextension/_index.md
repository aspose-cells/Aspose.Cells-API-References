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
[Test]
        public void Property_WebExtension()
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

* class [WebExtension](../../../aspose.cells.webextensions/webextension/)
* class [WebExtensionShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


