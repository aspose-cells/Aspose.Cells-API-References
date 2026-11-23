---
title: "Énumération BubbleSizeRepresents"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.Charts.BubbleSizeRepresents. Représente ce que la taille de la bulle indique sur un graphique à bulles."
type: docs
url: /fr/net/aspose.cells.charts/bubblesizerepresents/
---
## BubbleSizeRepresents enumeration

Représente ce que la taille de la bulle indique sur un graphique à bulles.

```csharp
public enum BubbleSizeRepresents
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| SizeIsArea | `0` | Représente la valeur de [`BubbleSizes`](../series/bubblesizes/), qui est la surface de la bulle. |
| SizeIsWidth | `1` | Représente la valeur de [`BubbleSizes`](../series/bubblesizes/) qui est la largeur de la bulle. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class BubbleSizeRepresentsDemo
    {
        public static void BubbleSizeRepresentsExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le graphique à bulles
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["B2"].PutValue(3);
            worksheet.Cells["B3"].PutValue(4);
            worksheet.Cells["C1"].PutValue(5);
            worksheet.Cells["C2"].PutValue(10);
            worksheet.Cells["C3"].PutValue(15);

            // Ajouter un graphique à bulles à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Bubble, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ajouter des séries au graphique à bulles
            int seriesIndex = chart.NSeries.Add("A1:C3", true);
            Series series = chart.NSeries[seriesIndex];

            // Définir les valeurs X, les valeurs Y et les tailles des bulles
            series.XValues = "A1:A3";
            series.Values = "B1:B3";
            series.BubbleSizes = "C1:C3";

            // Définir la représentation de la taille des bulles
            series.SizeRepresents = BubbleSizeRepresents.SizeIsArea;

            // Enregistrez le classeur
            workbook.Save("BubbleSizeRepresentsExample.xlsx");
            workbook.Save("BubbleSizeRepresentsExample.pdf");

            // Définir la représentation de la taille des bulles
            series.SizeRepresents = BubbleSizeRepresents.SizeIsWidth;

            // Enregistrez le classeur
            workbook.Save("BubbleSizeRepresentsExample2.xlsx");
            workbook.Save("BubbleSizeRepresentsExample2.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


