---
title: "Series.DoughnutHoleSize"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété de Series. Retourne ou définit la taille du trou dans un groupe de diagramme en beignet. La taille du trou est exprimée en pourcentage de la taille du diagramme, entre 10 et 90 %"
type: docs
url: /fr/net/aspose.cells.charts/series/doughnutholesize/
---
## Series.DoughnutHoleSize property

Renvoie ou définit la taille du trou dans un groupe de graphique en anneau. La taille du trou est exprimée en pourcentage de la taille du graphique, entre 10 et 90 %.

```csharp
public int DoughnutHoleSize { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyDoughnutHoleSizeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Ajouter un graphique en anneau
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Définir la taille du trou du beignet (pourcentage du rayon du diagramme)
            chart.NSeries[0].DoughnutHoleSize = 25;

            // Enregistrez le classeur
            workbook.Save("DoughnutHoleSizeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


