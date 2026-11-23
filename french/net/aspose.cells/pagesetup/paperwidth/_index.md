---
title: "PageSetup.PaperWidth"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PageSetup. Obtient la largeur du papier en unités de pouces selon l'orientation de la page"
type: docs
url: /fr/net/aspose.cells/pagesetup/paperwidth/
---
## PageSetup.PaperWidth property

Obtient la largeur du papier en pouces, en fonction de l'orientation de la page.

```csharp
public double PaperWidth { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPaperWidthDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir des données d'exemple
            worksheet.Cells["A1"].PutValue("Sample Page Setup Demo");
            
            // Accéder à la PageSetup de la feuille de calcul
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Démontrez la propriété PaperWidth (lecture seule)
            Console.WriteLine("Paper Width: " + pageSetup.PaperWidth);
            
            // Pour changer la taille du papier, utilisez la propriété PaperSize à la place
            pageSetup.PaperSize = PaperSizeType.PaperLetter;
            Console.WriteLine("New Paper Width: " + pageSetup.PaperWidth);
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


