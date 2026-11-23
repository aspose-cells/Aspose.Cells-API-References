---
title: "Classe WebExtension"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.WebExtensions.WebExtension. Représente une instance d'Office Add-in"
type: docs
url: /fr/net/aspose.cells.webextensions/webextension/
---
## WebExtension class

Représente une instance de complément Office.

```csharp
public class WebExtension
```

## Propriétés

| Nom | Description |
| --- | --- |
| [AlterReferences](../../aspose.cells.webextensions/webextension/alterreferences/) { get; } | Obtient une liste de références alternatives. |
| [Bindings](../../aspose.cells.webextensions/webextension/bindings/) { get; } | Obtient toutes les relations de liaison entre un Office Add-in et les données du document. |
| [Id](../../aspose.cells.webextensions/webextension/id/) { get; set; } | Obtient et définit l'identifiant unique de l'instance Office Add-in dans le document actuel. |
| [IsFrozen](../../aspose.cells.webextensions/webextension/isfrozen/) { get; set; } | Indique si l'utilisateur peut interagir avec l'Office Add-in ou non. |
| [Properties](../../aspose.cells.webextensions/webextension/properties/) { get; } | Obtient toutes les propriétés de l'extension web. |
| [Reference](../../aspose.cells.webextensions/webextension/reference/) { get; } | Obtenez la référence principale d'un Office Add-in. |

### Exemples

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

### Voir aussi

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


