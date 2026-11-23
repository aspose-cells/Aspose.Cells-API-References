---
title: "DataLabels.ShowBubbleSize"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataLabels. Représente le comportement d'affichage de la valeur en pourcentage d'une étiquette de données d'un graphique spécifié. True affiche la valeur en pourcentage. False masque la valeur en pourcentage"
type: docs
url: /fr/net/aspose.cells.charts/datalabels/showbubblesize/
---
## DataLabels.ShowBubbleSize property

Représente le comportement d'affichage de la valeur en pourcentage de l'étiquette de données d'un graphique spécifié. Vrai affiche la valeur en pourcentage. Faux masque la valeur en pourcentage.

```csharp
public bool ShowBubbleSize { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyShowBubbleSizeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique à bulles
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["C1"].PutValue("Size");
            worksheet.Cells["C2"].PutValue(5);
            worksheet.Cells["C3"].PutValue(10);
            worksheet.Cells["C4"].PutValue(15);

            // Ajouter un graphique à bulles
            int chartIndex = worksheet.Charts.Add(ChartType.Bubble, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ajouter des séries au graphique
            int seriesIndex = chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Définir les tailles des bulles pour la série
            Series series = chart.NSeries[seriesIndex];
            series.BubbleSizes = "C2:C4";

            // Accéder aux DataLabels de la série
            DataLabels dataLabels = series.DataLabels;

            // Démontrer la propriété ShowBubbleSize
            dataLabels.ShowBubbleSize = true; // Show bubble size in data labels
            dataLabels.ShowValue = true;      // Also show values for clarity

            // Enregistrez le classeur
            workbook.Save("DataLabelsShowBubbleSizeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


