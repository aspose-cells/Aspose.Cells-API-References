---
title: "SparklineGroupCollection.ClearSparklineGroups"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SparklineGroupCollection. Efface les groupes Sparkline qui chevauchent une zone de cellules"
type: docs
url: /fr/net/aspose.cells.charts/sparklinegroupcollection/clearsparklinegroups/
---
## SparklineGroupCollection.ClearSparklineGroups method

Efface les groupes de sparkline qui se chevauchent avec une zone de cellules.

```csharp
public void ClearSparklineGroups(CellArea cellArea)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| cellArea | CellArea | Spécifie la zone de cellules |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineGroupCollectionMethodClearSparklineGroupsWithCellAreaDemo
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


            try
            {
                // Appelez la méthode ClearSparklineGroups avec le paramètre CellArea
                sheet.SparklineGroups.ClearSparklineGroups(ca);
                
                Console.WriteLine("Sparkline groups cleared successfully for the specified cell area.");
                
                // Vérifiez le nombre de groupes Sparkline après le nettoyage
                Console.WriteLine($"Remaining sparkline groups count: {sheet.SparklineGroups.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearSparklineGroups method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("ClearSparklineGroupsWithCellAreaDemo.xlsx");
        }
    }
}
```

### Voir aussi

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


