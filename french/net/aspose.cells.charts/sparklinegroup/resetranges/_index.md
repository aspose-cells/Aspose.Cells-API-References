---
title: "SparklineGroup.ResetRanges"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SparklineGroup. Réinitialise la plage de données et la plage d'emplacement du groupe de sparklines. Cette méthode effacera les éléments sparkline originaux du groupe et créera de nouveaux éléments sparkline pour les nouvelles plages"
type: docs
url: /fr/net/aspose.cells.charts/sparklinegroup/resetranges/
---
## SparklineGroup.ResetRanges method

Réinitialise la plage de données et la plage d'emplacement du groupe de sparklines. Cette méthode effacera les éléments de sparkline d'origine dans le groupe et créera de nouveaux éléments de sparkline pour les nouvelles plages.

```csharp
public void ResetRanges(string dataRange, bool isVertical, CellArea locationRange)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| dataRange | String | Spécifie la nouvelle plage de données du groupe de sparklines. |
| isVertical | Boolean | Spécifie s'il faut tracer les sparklines de la nouvelle plage de données par ligne ou par colonne. |
| locationRange | CellArea | Spécifie où placer les sparklines. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineGroupMethodResetRangesWithStringBooleanCellAreaDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des données à la feuille de calcul
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Définit la CellArea pour le sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Ajoute un groupe de sparklines à la feuille de calcul
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);

            SparklineGroup group = sheet.SparklineGroups[idx];

            // Préparer les paramètres pour ResetRanges
            string dataRange = "A1:D1";
            bool isVertical = false;
            CellArea locationRange = CellArea.CreateCellArea(6, 5, 6, 5);

            try
            {
                // Appeler ResetRanges avec les paramètres (String, Boolean, CellArea)
                group.ResetRanges(dataRange, isVertical, locationRange);

                Console.WriteLine("ResetRanges method executed successfully with parameters (String, Boolean, CellArea)");
                
                
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ResetRanges method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("SparklineGroupResetRangesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


