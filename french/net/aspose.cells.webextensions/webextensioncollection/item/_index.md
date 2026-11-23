---
title: "WebExtensionCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WebExtensionCollection. Obtient l'extension web à l'index spécifié"
type: docs
url: /fr/net/aspose.cells.webextensions/webextensioncollection/item/
---
## WebExtensionCollection indexer

Obtient l'extension web par l'index spécifique.

```csharp
public WebExtension this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice. |

### Valeur de retour

L'extension web.

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Obtenir la collection d'extensions web
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            
            // Ajouter une extension de lecteur vidéo web
            int index = webExtensions.Add();
            WebExtension webExt = webExtensions[index];
            webExt.Reference.Id = "youtube";
            webExt.Reference.StoreName = "youtube.com";
            webExt.Properties.Add("videoUrl", "https://www.youtube.com/watch?v=z0hFbzPPfm8");
            
            // Ajouter une forme pour contenir l'extension web
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            shapes.AddShape(MsoDrawingType.WebExtension, 0, 0, 410, 730, 0, 0);
            
            // Attribuer l'extension web à la forme
            WebExtensionShape wShape = (WebExtensionShape)shapes[0];
            wShape.WebExtension = webExt;
            
            // Enregistrez le classeur
            workbook.Save("WebExtensionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [WebExtension](../../webextension/)
* class [WebExtensionCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


