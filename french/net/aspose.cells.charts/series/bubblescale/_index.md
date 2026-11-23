---
title: "Series.BubbleScale"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété de la série. Obtient ou définit le facteur d'échelle pour les bulles dans le groupe de graphique spécifié. Il peut s'agir d'une valeur entière de 0 à 300 correspondant à un pourcentage de la taille par défaut. S'applique uniquement aux graphiques à bulles"
type: docs
url: /fr/net/aspose.cells.charts/series/bubblescale/
---
## Series.BubbleScale property

Obtient ou définit le facteur d'échelle des bulles dans le groupe de graphiques spécifié. Il peut s'agir d'une valeur entière de 0 (zéro) à 300, correspondant à un pourcentage de la taille par défaut. S'applique uniquement aux graphiques à bulles.

```csharp
public int BubbleScale { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SeriesPropertyBubbleScaleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le graphique à bulles
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["C1"].PutValue("Size");
            
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["C2"].PutValue(5);
            
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["C3"].PutValue(10);
            
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["C4"].PutValue(15);

            // Ajouter un graphique à bulles
            int chartIndex = worksheet.Charts.Add(ChartType.Bubble, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ajouter des séries au graphique
            int seriesIndex = chart.NSeries.Add("B2:B4", true);
            chart.NSeries[seriesIndex].XValues = "A2:A4";
            chart.NSeries[seriesIndex].BubbleSizes = "C2:C4";
            
            // Définir l'échelle des bulles pour démontrer la propriété
            chart.NSeries[seriesIndex].BubbleScale = 150; // Scale bubbles to 150% of default size
            
            // Personnaliser l'apparence du graphique
            chart.Title.Text = "Bubble Chart with Scaled Bubbles";
            chart.NSeries[seriesIndex].Area.FillFormat.SetOneColorGradient(Color.LightBlue, 0.5, Aspose.Cells.Drawing.GradientStyleType.Horizontal, 1);
            
            // Enregistrez le classeur
            workbook.Save("BubbleScaleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


