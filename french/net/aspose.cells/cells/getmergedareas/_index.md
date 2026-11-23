---
title: "Cells.GetMergedAreas"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Récupère toutes les cellules fusionnées"
type: docs
url: /fr/net/aspose.cells/cells/getmergedareas/
---
## Cells.GetMergedAreas method

Obtient toutes les cellules fusionnées.

```csharp
public CellArea[] GetMergedAreas()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetMergedAreasDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer quelques cellules fusionnées
            worksheet.Cells.Merge(0, 0, 2, 2); // Merge A1:B2
            worksheet.Cells.Merge(3, 3, 3, 2); // Merge D4:E4
            worksheet.Cells.Merge(5, 0, 1, 5); // Merge A6:E6
            
            // Obtenir toutes les zones fusionnées
            CellArea[] mergedAreas = worksheet.Cells.GetMergedAreas();
            
            // Afficher les informations sur les zones fusionnées
            Console.WriteLine("Number of merged areas: " + mergedAreas.Length);
            foreach (CellArea area in mergedAreas)
            {
                Console.WriteLine($"Merged area: StartRow={area.StartRow}, StartColumn={area.StartColumn}, " +
                    $"EndRow={area.EndRow}, EndColumn={area.EndColumn}");
            }
        }
    }
}
```

### Voir aussi

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


