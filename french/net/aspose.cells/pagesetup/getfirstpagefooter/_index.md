---
title: "PageSetup.GetFirstPageFooter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PageSetup. Obtient un script formatant le pied de page de la première page d'un fichier Excel"
type: docs
url: /fr/net/aspose.cells/pagesetup/getfirstpagefooter/
---
## PageSetup.GetFirstPageFooter method

Obtient un script formatant le pied de page de la première page d'un fichier Excel.

```csharp
public string GetFirstPageFooter(int section)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| section | Int32 | 0 : Section gauche, 1 : Section centrale, 2 : Section droite. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodGetFirstPageFooterWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir le pied de page de la première page
            worksheet.PageSetup.SetFirstPageFooter(1, "First Page Footer");

            // Obtenir et imprimer le pied de page de la première page
            string footer = worksheet.PageSetup.GetFirstPageFooter(1);
            Console.WriteLine("First Page Footer: " + footer);

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


