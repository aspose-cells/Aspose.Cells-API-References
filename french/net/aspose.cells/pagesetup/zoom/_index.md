---
title: "PageSetup.Zoom"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PageSetup. Représente le facteur d'échelle en pourcentage. Il doit être compris entre 10 et 400"
type: docs
url: /fr/net/aspose.cells/pagesetup/zoom/
---
## PageSetup.Zoom property

Représente le facteur d'échelle en pourcentage. Il doit être compris entre 10 et 400.

```csharp
public int Zoom { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyZoomDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir le niveau de zoom à 150 %
            worksheet.PageSetup.Zoom = 150;
            
            // Imprimer le niveau de zoom actuel
            Console.WriteLine("Current Zoom Level: " + worksheet.PageSetup.Zoom);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


