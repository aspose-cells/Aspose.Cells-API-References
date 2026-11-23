---
title: "PageSetup.IsPercentScale"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PageSetup. Si cette propriété est False, les propriétés FitToPagesWide et FitToPagesTall contrôlent la façon dont la feuille de calcul est mise à l'échelle"
type: docs
url: /fr/net/aspose.cells/pagesetup/ispercentscale/
---
## PageSetup.IsPercentScale property

Si cette propriété est False, les propriétés FitToPagesWide et FitToPagesTall contrôlent la façon dont la feuille de calcul est mise à l'échelle.

```csharp
public bool IsPercentScale { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsPercentScaleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accéder à PageSetup et définir l'échelle à 80% (échelle en pourcentage)
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.Zoom = 80;
            pageSetup.IsPercentScale = true;

            // Afficher les paramètres pour démontrer IsPercentScale
            Console.WriteLine("Zoom: " + pageSetup.Zoom);
            Console.WriteLine("IsPercentScale: " + pageSetup.IsPercentScale);

            // Enregistrez le classeur
            workbook.Save("PageSetup_IsPercentScale_Output.xlsx");
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


