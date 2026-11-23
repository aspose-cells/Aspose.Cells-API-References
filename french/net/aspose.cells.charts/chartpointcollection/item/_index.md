---
title: "ChartPointCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ChartPointCollection propriété. Obtient l'élément ChartPoint à l'index spécifié dans la série"
type: docs
url: /fr/net/aspose.cells.charts/chartpointcollection/item/
---
## ChartPointCollection indexer

Obtient l'élément [`ChartPoint`](../../chartpoint/) à l'index spécifié dans la série.

```csharp
public ChartPoint this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'index du point du graphique dans la série. |

### Valeur de retour

L'objet ChartPoint.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPointCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Ajoutez un graphique
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accédez à un point de graphique spécifique en utilisant la propriété Item
            ChartPoint point = chart.NSeries[0].Points[1];
            
            // Modifiez le motif de remplissage du point
            point.Area.FillFormat.Pattern = FillPattern.LightHorizontal;

            // Enregistrez le classeur
            workbook.Save("ChartPointCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartPoint](../../chartpoint/)
* class [ChartPointCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


