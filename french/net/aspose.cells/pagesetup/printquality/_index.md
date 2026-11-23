---
title: "PageSetup.PrintQuality"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PageSetup. Représente la qualité d'impression"
type: docs
url: /fr/net/aspose.cells/pagesetup/printquality/
---
## PageSetup.PrintQuality property

Représente la qualité d'impression.

```csharp
public int PrintQuality { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintQualityDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir la qualité d'impression à 144 dpi
            worksheet.PageSetup.PrintQuality = 144;
            
            // Imprimer le réglage actuel de la qualité d'impression
            Console.WriteLine("Print Quality: " + worksheet.PageSetup.PrintQuality);
            
            // Enregistrez le classeur
            workbook.Save("PrintQualityDemo.xls");
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


