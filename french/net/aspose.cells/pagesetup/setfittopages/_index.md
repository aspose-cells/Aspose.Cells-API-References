---
title: "PageSetup.SetFitToPages"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PageSetup. Définit le nombre de pages auquel la feuille de calcul sera mise à l'échelle lors de l'impression"
type: docs
url: /fr/net/aspose.cells/pagesetup/setfittopages/
---
## PageSetup.SetFitToPages method

Définit le nombre de pages auquel la feuille de calcul sera mise à l'échelle lors de l'impression.

```csharp
public void SetFitToPages(int wide, int tall)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| large | Int32 | Pages en largeur. |
| haut | Int32 | Pages de hauteur. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetFitToPagesWithInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Accédez au PageSetup de la première feuille de calcul
            PageSetup setup = workbook.Worksheets[0].PageSetup;
            
            // Définir les paramètres d'ajustement aux pages
            setup.SetFitToPages(2, 3);
            
            // Vérifier et afficher les paramètres
            Console.WriteLine("IsPercentScale: " + setup.IsPercentScale);
            Console.WriteLine("FitToPagesWide: " + setup.FitToPagesWide);
            Console.WriteLine("FitToPagesTall: " + setup.FitToPagesTall);
            
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


