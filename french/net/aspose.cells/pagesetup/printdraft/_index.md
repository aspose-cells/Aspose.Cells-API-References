---
title: "PageSetup.PrintDraft"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PageSetup. Représente si la feuille sera imprimée sans graphiques"
type: docs
url: /fr/net/aspose.cells/pagesetup/printdraft/
---
## PageSetup.PrintDraft property

Représente si la feuille sera imprimée sans graphiques.

```csharp
public bool PrintDraft { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintDraftDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accéder à l'objet PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // Définir la propriété PrintDraft sur true
            pageSetup.PrintDraft = true;
            Console.WriteLine("PrintDraft set to: " + pageSetup.PrintDraft);

            // Modifier la propriété PrintDraft en false
            pageSetup.PrintDraft = false;
            Console.WriteLine("PrintDraft changed to: " + pageSetup.PrintDraft);

            // Enregistrez le classeur
            workbook.Save("PageSetup_PrintDraft_Example.xlsx");
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


