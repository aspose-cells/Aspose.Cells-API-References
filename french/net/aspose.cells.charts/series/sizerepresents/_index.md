---
title: "Series.SizeRepresents"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Series. Obtient ou définit ce que représente la taille de la bulle sur un graphique à bulles"
type: docs
url: /fr/net/aspose.cells.charts/series/sizerepresents/
---
## Series.SizeRepresents property

Obtient ou définit ce que représente la taille de la bulle dans un graphique à bulles.

```csharp
public BubbleSizeRepresents SizeRepresents { get; set; }
```

### Remarques

BubbleSizeRepresents.SizeIsArea signifie que la valeur [`BubbleSizes`](../bubblesizes/) est la surface de la bulle. BubbleSizeRepresents.SizeIsWidth signifie que la valeur [`BubbleSizes`](../bubblesizes/) est la largeur de la bulle.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertySizeRepresentsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique à bulles
            sheet.Cells["A1"].PutValue("X");
            sheet.Cells["B1"].PutValue("Y");
            sheet.Cells["C1"].PutValue("Size");
            for (int i = 2; i <= 5; i++)
            {
                sheet.Cells["A" + i].PutValue(i);
                sheet.Cells["B" + i].PutValue(i * 2);
                sheet.Cells["C" + i].PutValue(i * 0.5);
            }

            // Ajouter un graphique à bulles
            int chartIndex = sheet.Charts.Add(ChartType.Bubble, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // Définir les données de la série
            SeriesCollection series = chart.NSeries;
            series.Add("B2:B5", true);
            series.CategoryData = "A2:A5";
            series[0].BubbleSizes = "C2:C5";

            // Définir la propriété SizeRepresents
            series[0].SizeRepresents = BubbleSizeRepresents.SizeIsArea;

            // Enregistrez le classeur
            workbook.Save("SeriesPropertySizeRepresentsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [BubbleSizeRepresents](../../bubblesizerepresents/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


