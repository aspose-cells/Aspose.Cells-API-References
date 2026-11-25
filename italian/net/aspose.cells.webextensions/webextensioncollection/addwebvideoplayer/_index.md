---
title: "WebExtensionCollection.AddWebVideoPlayer"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo WebExtensionCollection. Aggiunge un lettore video web in Excel"
type: docs
url: /it/net/aspose.cells.webextensions/webextensioncollection/addwebvideoplayer/
---
## WebExtensionCollection.AddWebVideoPlayer method

Aggiunge un lettore video web in Excel.

```csharp
public int AddWebVideoPlayer(string url, bool autoPlay, int startTime, int endTime)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| url | String |  |
| autoPlay | Booleano | Indica se il video viene riprodotto automaticamente. |
| startTime | Int32 | Il tempo di inizio in unità di secondi. |
| endTime | Int32 | Il tempo di fine in unità di secondi. |

### Esempi

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

### Vedi anche

* class [WebExtensionCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


