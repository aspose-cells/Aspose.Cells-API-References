---
title: "Worksheet.GetSelectedAreas"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Worksheet. Obtient les plages de cellules sélectionnées dans la feuille de calcul du concepteur"
type: docs
url: /fr/net/aspose.cells/worksheet/getselectedareas/
---
## Worksheet.GetSelectedAreas method

Obtient les plages de cellules sélectionnées dans la feuille de calcul du concepteur.

```csharp
public Range[] GetSelectedAreas()
```

### Valeur de retour

Retourne toutes les plages sélectionnées.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodGetSelectedAreasDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Sélectionner plusieurs plages
            worksheet.SelectRange(0, 0, 2, 2, false); // First range (A1:C3)
            worksheet.SelectRange(4, 4, 6, 6, false); // Second range (E5:G7)
            
            // Obtenir les zones sélectionnées
            Aspose.Cells.Range[] selectedAreas = worksheet.GetSelectedAreas();
            
            // Afficher les informations sur les zones sélectionnées
            Console.WriteLine("Number of selected areas: " + selectedAreas.Length);
            for (int i = 0; i < selectedAreas.Length; i++)
            {
                Console.WriteLine($"Area {i + 1}: {selectedAreas[i].Address}");
            }
            
            // Effacer les sélections et sélectionner une seule plage
            worksheet.SelectRange(1, 1, 3, 3, true); // New single selection (B2:D4)
            
            // Obtenir la zone sélectionnée unique
            selectedAreas = worksheet.GetSelectedAreas();
            Console.WriteLine("\nAfter single selection:");
            Console.WriteLine("Number of selected areas: " + selectedAreas.Length);
            Console.WriteLine("Selected area: " + selectedAreas[0].Address);
        }
    }
}
```

### Voir aussi

* class [Range](../../range/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


