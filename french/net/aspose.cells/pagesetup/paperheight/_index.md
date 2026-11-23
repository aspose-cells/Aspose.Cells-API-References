---
title: "PageSetup.PaperHeight"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PageSetup. Obtient la hauteur du papier en pouces, en tenant compte de l'orientation de la page"
type: docs
url: /fr/net/aspose.cells/pagesetup/paperheight/
---
## PageSetup.PaperHeight property

Obtient la hauteur du papier en pouces, en fonction de l'orientation de la page.

```csharp
public double PaperHeight { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPaperHeightDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir des données dans une cellule
            worksheet.Cells["A1"].PutValue("Paper Height Demo");
            
            // Obtenir l'objet PageSetup
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Afficher la hauteur de papier par défaut (en pouces)
            Console.WriteLine("Default Paper Height: " + pageSetup.PaperHeight);
            
            // PaperHeight est en lecture seule, nous montrons donc comment obtenir différentes tailles de papier
            // en changeant le type de taille de papier à Letter (8,5 x 11 pouces)
            pageSetup.PaperSize = PaperSizeType.PaperLetter;
            
            // Vérifier le changement
            Console.WriteLine("Modified Paper Height (Letter size): " + pageSetup.PaperHeight);
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


