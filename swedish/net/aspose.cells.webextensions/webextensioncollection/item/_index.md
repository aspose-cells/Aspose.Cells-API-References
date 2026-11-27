---
title: "WebExtensionCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebExtensionCollection egenskap. Hämtar webbtillägg med det specifika indexet"
type: docs
url: /sv/net/aspose.cells.webextensions/webextensioncollection/item/
---
## WebExtensionCollection indexer

Hämtar web extension efter det specifika indexet.

```csharp
public WebExtension this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Indexet. |

### Returvärde

Webbtillägget.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Hämta samlingen av webbtillägg
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            
            // Lägg till ett webbvideospelartillägg
            int index = webExtensions.Add();
            WebExtension webExt = webExtensions[index];
            webExt.Reference.Id = "youtube";
            webExt.Reference.StoreName = "youtube.com";
            webExt.Properties.Add("videoUrl", "https://www.youtube.com/watch?v=z0hFbzPPfm8");
            
            // Lägg till en form för att hålla webbtillägget
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            shapes.AddShape(MsoDrawingType.WebExtension, 0, 0, 410, 730, 0, 0);
            
            // Tilldela webbtillägget till formen
            WebExtensionShape wShape = (WebExtensionShape)shapes[0];
            wShape.WebExtension = webExt;
            
            // Spara arbetsboken
            workbook.Save("WebExtensionDemo.xlsx");
        }
    }
}
```

### Se även

* class [WebExtension](../../webextension/)
* class [WebExtensionCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


