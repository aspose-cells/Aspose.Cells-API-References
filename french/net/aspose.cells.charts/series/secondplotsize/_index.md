---
title: "Series.SecondPlotSize"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété de Series. Retourne ou définit la taille de la section secondaire d'un diagramme en secteurs imbriqués ou d'un graphique en barres de secteurs, exprimée en pourcentage de la taille du secteur principal. Peut être une valeur de 5 à 200"
type: docs
url: /fr/net/aspose.cells.charts/series/secondplotsize/
---
## Series.SecondPlotSize property

Renvoie ou définit la taille de la section secondaire d'un graphique en secteurs de secteurs ou d'un graphique en barres de secteurs, en pourcentage de la taille du secteur principal. Peut être une valeur de 5 à 200.

```csharp
public short SecondPlotSize { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertySecondPlotSizeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le diagramme circulaire
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Ajouter un graphique en secteurs
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Obtenir la première série
            Series series = chart.NSeries[0];

            // Définir la propriété SecondPlotSize (pourcentage du secteur à afficher dans le deuxième tracé)
            series.SecondPlotSize = 30; // 30% of the pie will be shown in second plot

            // Enregistrez le classeur
            workbook.Save("SeriesPropertySecondPlotSizeDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


