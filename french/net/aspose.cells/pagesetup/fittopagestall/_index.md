---
title: "PageSetup.FitToPagesTall"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PageSetup. Représente le nombre de pages en hauteur auquel la feuille sera mise à l'échelle lors de l'impression. La valeur par défaut est 1"
type: docs
url: /fr/net/aspose.cells/pagesetup/fittopagestall/
---
## PageSetup.FitToPagesTall property

Représente le nombre de pages en hauteur auquel la feuille de calcul sera mise à l'échelle lors de l'impression. La valeur par défaut est 1.

```csharp
public int FitToPagesTall { get; set; }
```

### Remarques

Vous devez définir FitToPagesWide à zéro si vous souhaitez faire tenir toutes les lignes sur une seule page.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyFitToPagesTallDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour que la feuille s'étende sur plusieurs pages
            for (int i = 0; i < 100; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Row {i+1}, Col {j+1}");
                }
            }

            // Obtenir l'objet PageSetup
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Définir la zone d'impression
            pageSetup.PrintArea = "A1:J100";
            
            // Définir la propriété FitToPagesTall pour ajuster toutes les lignes sur une page
            pageSetup.FitToPagesTall = 1;
            
            // Définir la propriété FitToPagesWide pour ajuster toutes les colonnes sur une page
            pageSetup.FitToPagesWide = 1;
            
            // Définir la taille du papier
            pageSetup.PaperSize = PaperSizeType.PaperLetter;
            
            // Imprimer les lignes de grille
            pageSetup.PrintGridlines = true;

            // Créer des options de rendu
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // Créer un rendu de feuille
            SheetRender render = new SheetRender(worksheet, options);
            
            // Afficher l'échelle de la page
            Console.WriteLine($"Page scale: {Math.Round(render.PageScale, 2)}");
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


