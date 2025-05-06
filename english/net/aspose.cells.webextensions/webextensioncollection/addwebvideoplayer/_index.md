---
title: WebExtensionCollection.AddWebVideoPlayer
second_title: Aspose.Cells for .NET API Reference
description: WebExtensionCollection method. Add a web video player into exel
type: docs
url: /net/aspose.cells.webextensions/webextensioncollection/addwebvideoplayer/
---
## WebExtensionCollection.AddWebVideoPlayer method

Add a web video player into exel.

```csharp
public int AddWebVideoPlayer(string url, bool autoPlay, int startTime, int endTime)
```

| Parameter | Type | Description |
| --- | --- | --- |
| url | String |  |
| autoPlay | Boolean | Indicates whether auto playing the video. |
| startTime | Int32 | The start time in unit of seconds. |
| endTime | Int32 | The end time in unit of seconds. |

### Examples

```csharp
// Called: int index = webExtensions.AddWebVideoPlayer(&amp;quot;https://www.youtube.com/watch?v=z0hFbzPPfm8&amp;quot;, true, 0, 0);
[Test]
        public void Method_Int32_()
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

* class [WebExtensionCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


