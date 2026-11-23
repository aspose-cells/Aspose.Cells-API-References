---
title: "SparklineCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "propriété SparklineCollection. Obtient l'élément Sparkline à l'index spécifié"
type: docs
url: /fr/net/aspose.cells.charts/sparklinecollection/item/
---
## SparklineCollection indexer

Obtient l'élément [`Sparkline`](../../sparkline/) à l'index spécifié.

```csharp
public Sparkline this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice à base zéro de l'élément. |

### Valeur de retour

L’élément à l’index spécifié.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(3);
            worksheet.Cells["C1"].PutValue(7);
            worksheet.Cells["D1"].PutValue(2);

            // Créer un groupe de sparkline
            SparklineGroupCollection sparklineGroups = worksheet.SparklineGroups;
            int idx = sparklineGroups.Add(SparklineType.Line, "A1:D1", false, CellArea.CreateCellArea(0, 4, 0, 4));
            SparklineGroup group = sparklineGroups[idx];

            // Accédez aux sparklines en utilisant la propriété Item
            Sparkline sparkline = group.Sparklines[0];
            Console.WriteLine("Sparkline Data Range: " + sparkline.DataRange);
            Console.WriteLine("Sparkline Type: " + group.Type);

            // Modifier les données du sparkline
            worksheet.Cells["A1"].PutValue(8);
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Sparkline](../../sparkline/)
* class [SparklineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


