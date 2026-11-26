---
title: "WebExtensionCollection.AddWebVideoPlayer"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método WebExtensionCollection. Agrega un reproductor de video web en Excel"
type: docs
url: /es/net/aspose.cells.webextensions/webextensioncollection/addwebvideoplayer/
---
## WebExtensionCollection.AddWebVideoPlayer method

Agrega un reproductor de video web en exel.

```csharp
public int AddWebVideoPlayer(string url, bool autoPlay, int startTime, int endTime)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| url | String |  |
| autoPlay | Booleano | Indica si el video se reproduce automáticamente. |
| startTime | Int32 | El tiempo de inicio en unidades de segundos. |
| endTime | Int32 | El tiempo de finalización en unidades de segundos. |

### Ejemplos

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

### Ver también

* class [WebExtensionCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


