---
title: "SparklineCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "SparklineCollection method. Ajoutez un sparkline"
type: docs
url: /fr/net/aspose.cells.charts/sparklinecollection/add/
---
## SparklineCollection.Add method

Ajoute un sparkline.

```csharp
public int Add(string dataRange, int row, int column)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| dataRange | String | Spécifie la nouvelle plage de données du sparkline. |
| ligne | Int32 | L'index de ligne de l'emplacement. |
| column | Int32 | L'index de colonne de l'emplacement. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineCollectionMethodAddWithStringInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            for (int i = 0; i < 12; i++)
            {
                worksheet.Cells[4, 3 + i].PutValue(i + 1);
            }

            // Créer un groupe de sparkline
            int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Line);
            SparklineGroup group = worksheet.SparklineGroups[groupIndex];

            // Ajouter un sparkline avec la plage de données et l'emplacement
            int sparklineIndex = group.Sparklines.Add("D5:O5", 4, 15);

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [SparklineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


