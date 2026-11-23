---
title: "Series.BubbleSizes"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Series. Obtient ou définit les valeurs de taille des bulles de la série de graphique"
type: docs
url: /fr/net/aspose.cells.charts/series/bubblesizes/
---
## Series.BubbleSizes property

Obtient ou définit les valeurs de taille des bulles de la série du graphique.

```csharp
public string BubbleSizes { get; set; }
```

### Remarques

Uniquement pour Bubble ou Bubble3D.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyBubbleSizesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique à bulles
            worksheet.Cells["A1"].PutValue("X Values");
            worksheet.Cells["B1"].PutValue("Y Values");
            worksheet.Cells["C1"].PutValue("Bubble Sizes");
            
            for (int i = 2; i <= 5; i++)
            {
                worksheet.Cells["A" + i].PutValue(i);
                worksheet.Cells["B" + i].PutValue(i * 2);
                worksheet.Cells["C" + i].PutValue(i * 0.5);
            }

            // Ajouter un graphique à bulles
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Bubble, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Définissez les données de la série en utilisant la propriété BubbleSizes
            chart.NSeries.Add("A2:A5", true);
            chart.NSeries[0].XValues = "B2:B5";
            chart.NSeries[0].BubbleSizes = "C2:C5";

            // Enregistrez le classeur
            workbook.Save("BubbleChartDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


