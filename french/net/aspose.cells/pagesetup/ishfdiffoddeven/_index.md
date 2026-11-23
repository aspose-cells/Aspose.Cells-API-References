---
title: "PageSetup.IsHFDiffOddEven"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PageSetup. True signifie que l'en-tête/pied de page des pages impaires est différent de celui des pages paires"
type: docs
url: /fr/net/aspose.cells/pagesetup/ishfdiffoddeven/
---
## PageSetup.IsHFDiffOddEven property

True signifie que l'en-tête/pied de page des pages impaires est différent avec les pages impaires.

```csharp
public bool IsHFDiffOddEven { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsHFDiffOddEvenDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accédez à PageSetup
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Activer des en-têtes/pieds de page différents pour les pages impaires et paires
            pageSetup.IsHFDiffOddEven = true;
            
            // Définir des pieds de page différents pour les pages impaires et paires
            pageSetup.SetFooter(0, "Odd Page Footer");
            pageSetup.SetEvenFooter(0, "Even Page Footer");
            
            // Enregistrez le classeur
            workbook.Save("PageSetup_IsHFDiffOddEven_Example.xlsx");
            
            // Vérifier les paramètres en chargeant le fichier enregistré
            Workbook loadedWorkbook = new Workbook("PageSetup_IsHFDiffOddEven_Example.xlsx");
            PageSetup loadedPageSetup = loadedWorkbook.Worksheets[0].PageSetup;
            
            Console.WriteLine("IsHFDiffOddEven: " + loadedPageSetup.IsHFDiffOddEven);
            Console.WriteLine("Odd Page Footer: " + loadedPageSetup.GetFooter(0));
            Console.WriteLine("Even Page Footer: " + loadedPageSetup.GetEvenFooter(0));
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


