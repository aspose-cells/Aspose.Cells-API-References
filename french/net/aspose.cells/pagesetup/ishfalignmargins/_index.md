---
title: "PageSetup.IsHFAlignMargins"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PageSetup. Indique si les marges d'en-tête et de pied de page sont alignées avec les marges de la page. Si cette propriété est vraie, l'en-tête et le pied de page gauche seront alignés avec la marge gauche et l'en-tête et le pied de page droit seront alignés avec la marge droite. Cette option est activée par défaut"
type: docs
url: /fr/net/aspose.cells/pagesetup/ishfalignmargins/
---
## PageSetup.IsHFAlignMargins property

Indique si les marges d'en-tête et de pied de page sont alignées avec les marges de la page. Si cette propriété est true, l'en-tête et le pied de page gauche seront alignés avec la marge gauche, et l'en-tête et le pied de page droit seront alignés avec la marge droite. Cette option est activée par défaut.

```csharp
public bool IsHFAlignMargins { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsHFAlignMarginsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accéder à la PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // Définir IsHFAlignMargins sur true
            pageSetup.IsHFAlignMargins = true;
            Console.WriteLine("IsHFAlignMargins set to: " + pageSetup.IsHFAlignMargins);

            // Modifier IsHFAlignMargins sur false
            pageSetup.IsHFAlignMargins = false;
            Console.WriteLine("IsHFAlignMargins changed to: " + pageSetup.IsHFAlignMargins);

            // Enregistrez le classeur
            workbook.Save("PageSetup_IsHFAlignMargins_Example.xlsx");
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


