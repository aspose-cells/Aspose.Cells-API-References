---
title: "SparklineGroupCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SparklineGroupCollection. Obtient l'élément SparklineGroup à l'index spécifié"
type: docs
url: /fr/net/aspose.cells.charts/sparklinegroupcollection/item/
---
## SparklineGroupCollection indexer

Obtient l'élément [`SparklineGroup`](../../sparklinegroup/) à l'index spécifié.

```csharp
public SparklineGroup this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice à base zéro de l'élément. |

### Valeur de retour

L’élément à l’index spécifié.

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Ajoutez des données d'exemple
            ws.Cells["A1"].PutValue(5);
            ws.Cells["A2"].PutValue(3);
            ws.Cells["A3"].PutValue(7);
            ws.Cells["A4"].PutValue(2);
            ws.Cells["A5"].PutValue(9);

            // Définir la plage de données et l'emplacement pour les sparklines
            string dataRange = "'" + ws.Name + "'!A1:A5";
            CellArea location = new CellArea();
            location.StartRow = 0;
            location.EndRow = 0;
            location.StartColumn = 1;
            location.EndColumn = 1;

            // Ajouter un groupe de sparkline
            int index = ws.SparklineGroups.Add(SparklineType.Line, dataRange, false, location);
            
            // Accédez au groupe de sparkline en utilisant la propriété Item
            SparklineGroup group = ws.SparklineGroups[index];
            
            // Personnalisez le sparkline
            CellsColor color = wb.CreateCellsColor();
            color.Color = Color.Blue;
            group.SeriesColor = color;

            // Enregistrez le classeur
            wb.Save("SparklineGroupCollectionPropertyItemDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [SparklineGroup](../../sparklinegroup/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


