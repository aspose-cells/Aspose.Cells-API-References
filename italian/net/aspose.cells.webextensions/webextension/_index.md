---
title: "Classe WebExtension"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.WebExtensions.WebExtension. Rappresenta un'istanza di Office Add-in"
type: docs
url: /it/net/aspose.cells.webextensions/webextension/
---
## WebExtension class

Rappresenta un'istanza di Office Add-in.

```csharp
public class WebExtension
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AlterReferences](../../aspose.cells.webextensions/webextension/alterreferences/) { get; } | Ottiene un elenco di alter references. |
| [Bindings](../../aspose.cells.webextensions/webextension/bindings/) { get; } | Ottiene tutte le relazioni di binding tra un Office Add-in e i dati nel documento. |
| [Id](../../aspose.cells.webextensions/webextension/id/) { get; set; } | Ottiene e imposta l'identificatore univoco dell'istanza di Office Add-in nel documento corrente. |
| [IsFrozen](../../aspose.cells.webextensions/webextension/isfrozen/) { get; set; } | Indica se l'utente può interagire con l'Office Add-in o meno. |
| [Properties](../../aspose.cells.webextensions/webextension/properties/) { get; } | Ottiene tutte le proprietà dell'estensione web. |
| [Reference](../../aspose.cells.webextensions/webextension/reference/) { get; } | Ottieni il riferimento primario a un Office Add-in. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionsClassWebExtensionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int index = webExtensions.Add();
            WebExtension webExt = webExtensions[index];
            webExt.Reference.Id = "youtube";
            webExt.Reference.StoreName = "YouTube";
            
            webExt.Properties.Add("videoUrl", "https://www.youtube.com/watch?v=z0hFbzPPfm8");
            
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            shapes.AddShape(MsoDrawingType.WebExtension, 0, 0, 0, 0, 410, 730);
            WebExtensionShape wShape = (WebExtensionShape)shapes[0];
            wShape.WebExtension = webExt;
            
            workbook.Save("WebExtensionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


