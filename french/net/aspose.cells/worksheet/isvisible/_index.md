---
title: "Worksheet.IsVisible"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Représente si la feuille de calcul est visible"
type: docs
url: /fr/net/aspose.cells/worksheet/isvisible/
---
## Worksheet.IsVisible property

Représente si la feuille de calcul est visible.

```csharp
public bool IsVisible { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter 3 feuilles de calcul
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // Définir la deuxième feuille de calcul comme masquée
            workbook.Worksheets[1].IsVisible = false;
            
            // Enregistrez le classeur
            workbook.Save("WorksheetVisibilityDemo.xlsx");
            
            // Afficher l'état de visibilité
            Console.WriteLine("Worksheet Visibility Status:");
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Console.WriteLine($"{workbook.Worksheets[i].Name}: {(workbook.Worksheets[i].IsVisible ? "Visible" : "Hidden")}");
            }
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


