---
title: "PaginatedSaveOptions.DrawObjectEventHandler"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PaginatedSaveOptions. Implémente cette interface pour obtenir DrawObject et Bound lors du rendu"
type: docs
url: /fr/net/aspose.cells/paginatedsaveoptions/drawobjecteventhandler/
---
## PaginatedSaveOptions.DrawObjectEventHandler property

Implémentez cette interface pour obtenir DrawObject et Bound lors du rendu.

```csharp
public DrawObjectEventHandler DrawObjectEventHandler { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PaginatedSaveOptionsPropertyDrawObjectEventHandlerDemo
    {
        private class CustomDrawObjectEventHandler : DrawObjectEventHandler
        {
            public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
            {
                Console.WriteLine($"DrawObject Type: {drawObject.Type}");
                Console.WriteLine($"Position: X={x}, Y={y}, Width={width}, Height={height}");
            }
        }

        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple et des formes
            worksheet.Cells["A1"].PutValue("Test DrawObjectEventHandler");
            worksheet.Cells["A2"].PutValue("This will demonstrate the event handler during rendering");
            
            // Créez une instance d'options d'enregistrement paginées
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Affichez la valeur actuelle de la propriété (devrait être null initialement)
            Console.WriteLine("Current DrawObjectEventHandler value: " + (saveOptions.DrawObjectEventHandler == null ? "null" : "assigned"));
            
            // Définissez un nouveau gestionnaire d'événement personnalisé
            saveOptions.DrawObjectEventHandler = new CustomDrawObjectEventHandler();
            
            // Cela déclenchera la méthode Draw lors du rendu
            workbook.Save("PropertyDrawObjectEventHandlerDemo.pdf", saveOptions);
            
            // Changez le gestionnaire d'événement en null pour démontrer la différence
            saveOptions.DrawObjectEventHandler = null;
            workbook.Save("PropertyDrawObjectEventHandlerDemo_NoHandler.pdf", saveOptions);
        }
    }
}
```

### Voir aussi

* class [DrawObjectEventHandler](../../../aspose.cells.rendering/drawobjecteventhandler/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


