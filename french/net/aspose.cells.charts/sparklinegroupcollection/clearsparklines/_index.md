---
title: "SparklineGroupCollection.ClearSparklines"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SparklineGroupCollection. Supprime les sparklines qui se trouvent dans une zone de cellules"
type: docs
url: /fr/net/aspose.cells.charts/sparklinegroupcollection/clearsparklines/
---
## SparklineGroupCollection.ClearSparklines method

Efface les sparklines qui se trouvent à l'intérieur d'une zone de cellules.

```csharp
public void ClearSparklines(CellArea cellArea)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| cellArea | CellArea | Spécifie la zone de cellules |

### Remarques

[`SparklineGroup`](../../sparklinegroup/) will be removed too if it does not contains any [`Sparkline`](../../sparkline/).

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineGroupCollectionMethodClearSparklinesWithCellAreaDemo
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
                // Appelez la méthode ClearSparklines avec le paramètre CellArea
                sheet.SparklineGroups.ClearSparklines(ca);
                
                Console.WriteLine("Sparklines cleared successfully from the specified area.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearSparklines method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("SparklineGroupCollectionMethodClearSparklinesWithCellAreaDemo.xlsx");
        }
    }
}
```

### Voir aussi

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


