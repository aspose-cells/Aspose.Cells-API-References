---
title: "WebExtensionCollection.AddWebVideoPlayer"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebExtensionCollection metod. Lägg till en webbvideospelare i exel"
type: docs
url: /sv/net/aspose.cells.webextensions/webextensioncollection/addwebvideoplayer/
---
## WebExtensionCollection.AddWebVideoPlayer method

Lägg till en web video-spelare i exel.

```csharp
public int AddWebVideoPlayer(string url, bool autoPlay, int startTime, int endTime)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| url | String |  |
| autoPlay | Boolean | Anger om videon ska spelas upp automatiskt. |
| startTime | Int32 | Starttiden i sekunder. |
| endTime | Int32 | Sluttiden i sekunder. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionCollectionMethodAddWebVideoPlayerWithStringBooleanInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            
            int index = webExtensions.AddWebVideoPlayer(
                "https://www.youtube.com/watch?v=z0hFbzPPfm8", 
                true, 
                0, 
                0);
                
            WebExtension webExt = webExtensions[index];
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            shapes.AddShape(MsoDrawingType.WebExtension, 0, 0, 410, 730, 0, 0);
            
            WebExtensionShape wShape = (WebExtensionShape)shapes[0];
            wShape.WebExtension = webExt;
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [WebExtensionCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


