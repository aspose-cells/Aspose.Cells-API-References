---
title: "Cells.ClearMergedCells"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Efface toutes les plages fusionnées"
type: docs
url: /fr/net/aspose.cells/cells/clearmergedcells/
---
## Cells.ClearMergedCells method

Efface toutes les plages fusionnées.

```csharp
public void ClearMergedCells()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodClearMergedCellsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des cellules fusionnées dans A1:B2
            worksheet.Cells.Merge(0, 0, 2, 2);
            Console.WriteLine($"Merged areas before clearing: {worksheet.Cells.GetMergedAreas().Length}");

            try
            {
                // Effacer toutes les cellules fusionnées dans la feuille de calcul
                worksheet.Cells.ClearMergedCells();
                Console.WriteLine("Method executed successfully");
                Console.WriteLine($"Merged areas after clearing: {worksheet.Cells.GetMergedAreas().Length}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearMergedCells method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("ClearMergedCellsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


