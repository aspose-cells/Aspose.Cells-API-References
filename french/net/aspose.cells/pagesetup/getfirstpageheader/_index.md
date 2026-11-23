---
title: "PageSetup.GetFirstPageHeader"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PageSetup. Récupère un script formatant l'en-tête de la première page d'un fichier Excel"
type: docs
url: /fr/net/aspose.cells/pagesetup/getfirstpageheader/
---
## PageSetup.GetFirstPageHeader method

Obtient un script formatant l'en-tête de la première page d'un fichier Excel.

```csharp
public string GetFirstPageHeader(int section)
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
    public class PageSetupMethodGetFirstPageHeaderWithInt32Demo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accédez à PageSetup
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Activer un en-tête/pied de page différent pour la première page
            pageSetup.IsHFDiffFirst = true;
            
            // Définir les sections d'en-tête de la première page
            pageSetup.SetFirstPageHeader(0, "&LFirst Page Left Header");
            pageSetup.SetFirstPageHeader(1, "&CFirst Page Center Header");
            pageSetup.SetFirstPageHeader(2, "&RFirst Page Right Header");
            
            // Obtenir et afficher les sections d'en-tête de la première page
            Console.WriteLine("First Page Header Sections:");
            Console.WriteLine("Left: " + pageSetup.GetFirstPageHeader(0));
            Console.WriteLine("Center: " + pageSetup.GetFirstPageHeader(1));
            Console.WriteLine("Right: " + pageSetup.GetFirstPageHeader(2));
            
            // Enregistrez le classeur
            workbook.Save("PageSetupFirstPageHeaderDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


