---
title: "WebExtensionCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WebExtensionCollection. Ottiene l'estensione web per l'indice specifico"
type: docs
url: /it/net/aspose.cells.webextensions/webextensioncollection/item/
---
## WebExtensionCollection indexer

Ottiene l'estensione web per l'indice specifico.

```csharp
public WebExtension this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice. |

### Valore di ritorno

L'estensione web.

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Ottieni la raccolta di estensioni web
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            
            // Aggiungi un'estensione per il lettore video web
            int index = webExtensions.Add();
            WebExtension webExt = webExtensions[index];
            webExt.Reference.Id = "youtube";
            webExt.Reference.StoreName = "youtube.com";
            webExt.Properties.Add("videoUrl", "https://www.youtube.com/watch?v=z0hFbzPPfm8");
            
            // Aggiungi una forma per contenere l'estensione web
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            shapes.AddShape(MsoDrawingType.WebExtension, 0, 0, 410, 730, 0, 0);
            
            // Assegna l'estensione web alla forma
            WebExtensionShape wShape = (WebExtensionShape)shapes[0];
            wShape.WebExtension = webExt;
            
            // Salva la cartella di lavoro
            workbook.Save("WebExtensionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [WebExtension](../../webextension/)
* class [WebExtensionCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


