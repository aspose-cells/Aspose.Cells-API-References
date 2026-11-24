---
title: "WebExtensionCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebExtensionCollection-Eigenschaft. Gibt die Web-Erweiterung anhand des angegebenen Index zurück"
type: docs
url: /de/net/aspose.cells.webextensions/webextensioncollection/item/
---
## WebExtensionCollection indexer

Liefert die Web-Extension anhand des angegebenen Index.

```csharp
public WebExtension this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der Index. |

### Rückgabewert

Die Web-Erweiterung.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Holen Sie die Sammlung der Web-Erweiterungen
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            
            // Fügen Sie eine Web-Video-Player-Erweiterung hinzu
            int index = webExtensions.Add();
            WebExtension webExt = webExtensions[index];
            webExt.Reference.Id = "youtube";
            webExt.Reference.StoreName = "youtube.com";
            webExt.Properties.Add("videoUrl", "https://www.youtube.com/watch?v=z0hFbzPPfm8");
            
            // Fügen Sie eine Form hinzu, um die Web-Erweiterung zu halten
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            shapes.AddShape(MsoDrawingType.WebExtension, 0, 0, 410, 730, 0, 0);
            
            // Weisen Sie die Web-Erweiterung der Form zu
            WebExtensionShape wShape = (WebExtensionShape)shapes[0];
            wShape.WebExtension = webExt;
            
            // Speichere die Arbeitsmappe
            workbook.Save("WebExtensionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [WebExtension](../../webextension/)
* class [WebExtensionCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


