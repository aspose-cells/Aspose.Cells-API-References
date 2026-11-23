---
title: "PageSetup.GetEvenFooter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PageSetup. Obtient un script formatant le pied de page pair d'un fichier Excel"
type: docs
url: /fr/net/aspose.cells/pagesetup/getevenfooter/
---
## PageSetup.GetEvenFooter method

Obtient un script formatant le pied de page pair d'un fichier Excel.

```csharp
public string GetEvenFooter(int section)
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
    public class PageSetupMethodGetEvenFooterWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Activer des en-têtes/pieds de page différents pour les pages impaires et paires
            pageSetup.IsHFDiffOddEven = true;
            
            // Définir le pied de page pair
            pageSetup.SetEvenFooter(0, "Even Page Footer");
            
            // Obtenir et afficher le pied de page pair
            string evenFooter = pageSetup.GetEvenFooter(0);
            Console.WriteLine("Even Footer: " + evenFooter);
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


