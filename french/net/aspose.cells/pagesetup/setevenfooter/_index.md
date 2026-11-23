---
title: "PageSetup.SetEvenFooter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PageSetup. Définit un script formatant le pied de page pair d'un fichier Excel. Effet uniquement dans Excel 2007 lorsque IsHFDiffOddEven est true"
type: docs
url: /fr/net/aspose.cells/pagesetup/setevenfooter/
---
## PageSetup.SetEvenFooter method

Définit un script formatant le pied de page pair d'un fichier Excel. N'a d'effet que dans Excel 2007 lorsque IsHFDiffOddEven est vrai.

```csharp
public void SetEvenFooter(int section, string footerScript)
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
    public class PageSetupMethodSetEvenFooterWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Activer des en-têtes/pieds de page différents pour les pages première et paire
            pageSetup.IsHFDiffFirst = true;
            pageSetup.IsHFDiffOddEven = true;

            // Définir différents types de pied de page
            pageSetup.SetEvenFooter(0, "Even Page Footer");
            pageSetup.SetFooter(0, "Odd Page Footer");
            pageSetup.SetFirstPageFooter(0, "First Page Footer");

            // Enregistrez le classeur
            workbook.Save("PageSetup_SetEvenFooter_Example.xlsx");

            Console.WriteLine("Workbook saved with even page footer set successfully.");
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


