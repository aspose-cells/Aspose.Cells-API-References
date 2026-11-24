---
title: "WebExtensionCollection.AddWebVideoPlayer"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebExtensionCollection-Methode. Fügt einen Web-Video-Player in Excel ein"
type: docs
url: /de/net/aspose.cells.webextensions/webextensioncollection/addwebvideoplayer/
---
## WebExtensionCollection.AddWebVideoPlayer method

Füge einen Web-Video-Player in Excel ein.

```csharp
public int AddWebVideoPlayer(string url, bool autoPlay, int startTime, int endTime)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| URL | String |  |
| autoPlay | Boolean | Gibt an, ob das Video automatisch abgespielt wird. |
| startTime | Int32 | Die Startzeit in Sekunden. |
| endTime | Int32 | Die Endzeit in Sekunden. |

### Beispiele

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

### Siehe auch

* class [WebExtensionCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


