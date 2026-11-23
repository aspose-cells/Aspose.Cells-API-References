---
title: "PageSetup.IsHFDiffFirst"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PageSetup. True signifie que l'en-tête/pied de page de la première page est différent des autres pages"
type: docs
url: /fr/net/aspose.cells/pagesetup/ishfdifffirst/
---
## PageSetup.IsHFDiffFirst property

True signifie que l'en-tête/pied de page de la première page est différent des autres pages.

```csharp
public bool IsHFDiffFirst { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsHFDiffFirstDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accédez à PageSetup
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Définir des en-têtes/pieds de page différents pour la première page
            pageSetup.IsHFDiffFirst = true;
            
            // Définir les en-têtes/pieds de page
            pageSetup.SetFirstPageHeader(0, "First Page Header");
            pageSetup.SetHeader(0, "Standard Header");
            
            // Enregistrez le classeur
            workbook.Save("PageSetup_IsHFDiffFirst_Example.xlsx");
            
            // Recharger le classeur pour vérifier les paramètres
            Workbook loadedWorkbook = new Workbook("PageSetup_IsHFDiffFirst_Example.xlsx");
            PageSetup loadedPageSetup = loadedWorkbook.Worksheets[0].PageSetup;
            
            // Afficher la vérification
            Console.WriteLine("IsHFDiffFirst: " + loadedPageSetup.IsHFDiffFirst);
            Console.WriteLine("First Page Header: " + loadedPageSetup.GetFirstPageHeader(0));
            Console.WriteLine("Standard Header: " + loadedPageSetup.GetHeader(0));
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


