---
title: "PageSetup.SetFirstPageFooter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PageSetup. Définit un script formatant le pied de page de la première page d'un fichier Excel"
type: docs
url: /fr/net/aspose.cells/pagesetup/setfirstpagefooter/
---
## PageSetup.SetFirstPageFooter method

Définit un script formatant le pied de page de la première page d'un fichier Excel.

```csharp
public void SetFirstPageFooter(int section, string footerScript)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| section | Int32 | 0 : Section gauche, 1 : Section centrale, 2 : Section droite. |
| footerScript | String | Script de format du pied de page. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetFirstPageFooterWithInt32StringDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtenir l'objet PageSetup
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Définir des en-têtes/pieds de page différents pour la première page
            pageSetup.IsHFDiffFirst = true;
            
            // Définir le pied de page de la première page avec l'index de section et le texte
            pageSetup.SetFirstPageFooter(0, "First Page Footer Text");
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
            
            Console.WriteLine("First page footer set successfully.");
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


