---
title: "Worksheet.IsPageBreakPreview"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Indique si la feuille de calcul spécifiée est affichée en mode normal ou en aperçu des sauts de page"
type: docs
url: /fr/net/aspose.cells/worksheet/ispagebreakpreview/
---
## Worksheet.IsPageBreakPreview property

Indique si la feuille de calcul spécifiée est affichée en mode normal ou en aperçu des sauts de page.

```csharp
public bool IsPageBreakPreview { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsPageBreakPreviewDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définissez la feuille de calcul en mode aperçu des sauts de page
            worksheet.IsPageBreakPreview = true;
            
            // Définissez le zoom à 100 % pour la démonstration
            worksheet.Zoom = 100;
            
            // Affichez les paramètres actuels
            Console.WriteLine("IsPageBreakPreview: " + worksheet.IsPageBreakPreview);
            Console.WriteLine("Zoom: " + worksheet.Zoom);
            
            // Enregistrez le classeur
            workbook.Save("WorksheetPropertyIsPageBreakPreviewDemo_output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


