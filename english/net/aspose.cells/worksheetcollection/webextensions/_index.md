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

* class [WebExtensionCollection](../../../aspose.cells.webextensions/webextensioncollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


