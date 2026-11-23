---
title: "PageSetup.PrintCopies"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PageSetup. Récupère et définit le nombre de copies à imprimer"
type: docs
url: /fr/net/aspose.cells/pagesetup/printcopies/
---
## PageSetup.PrintCopies property

Obtient et définit le nombre de copies à imprimer.

```csharp
public int PrintCopies { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintCopiesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir le nombre de copies d'impression à 3
            worksheet.PageSetup.PrintCopies = 3;
            
            // Afficher le réglage actuel du nombre de copies d'impression
            Console.WriteLine("Print Copies: " + worksheet.PageSetup.PrintCopies);
            
            // Enregistrez le classeur
            workbook.Save("PageSetup_PrintCopies_Output.xlsx");
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


