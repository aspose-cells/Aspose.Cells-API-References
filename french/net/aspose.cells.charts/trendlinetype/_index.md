---
title: "Énumération TrendlineType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Charts.TrendlineType enum. Représente le type de ligne de tendance"
type: docs
url: /fr/net/aspose.cells.charts/trendlinetype/
---
## TrendlineType enumeration

Représente le type de ligne de tendance.

```csharp
public enum TrendlineType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Exponential | `0` | Exponentiel |
| Linear | `1` | Linéaire |
| Logarithmic | `2` | Logarithmique |
| MovingAverage | `3` | MoyenneMobile |
| Polynomial | `4` | Polynomial |
| Power | `5` | Puissance |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class TrendlineTypeDemo
    {
        public static void TrendlineTypeExample()
        {
            // Instanciation d'un objet Workbook
            Workbook workbook = new Workbook();
            
            // Ajout d'une nouvelle feuille de calcul à l'objet Excel
            int sheetIndex = workbook.Worksheets.Add();
            
            // Obtention de la référence de la feuille de calcul nouvellement ajoutée en passant son indice de feuille
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Ajout de valeurs d'exemple aux cellules
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Ajout d'un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            
            // Accès à l'instance du graphique nouvellement ajouté
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ajoute NSeries (source de données du graphique) au graphique allant de la cellule "A1" à "B4"
            chart.NSeries.Add("A1:B4", true);
            
            // Définir la source de données pour les données de catégorie de NSeries
            chart.NSeries.CategoryData = "C1:C4";

            // Ajout de différents types de lignes de tendance au graphique
            AddTrendline(chart, 0, TrendlineType.Linear, "Linear Trendline");
            AddTrendline(chart, 0, TrendlineType.Exponential, "Exponential Trendline");
            AddTrendline(chart, 0, TrendlineType.Logarithmic, "Logarithmic Trendline");
            AddTrendline(chart, 0, TrendlineType.MovingAverage, "Moving Average Trendline");
            AddTrendline(chart, 0, TrendlineType.Polynomial, "Polynomial Trendline");
            AddTrendline(chart, 0, TrendlineType.Power, "Power Trendline");

            // Enregistrement du fichier Excel
            workbook.Save("TrendlineTypeExample.xlsx");
        }

        private static void AddTrendline(Chart chart, int seriesIndex, TrendlineType trendlineType, string trendlineName)
        {
            // Ajout d'une ligne de tendance du type spécifié à la série spécifiée
            int index = chart.NSeries[seriesIndex].TrendLines.Add(trendlineType);
            Trendline trendline = chart.NSeries[seriesIndex].TrendLines[index];
            
            // Définition du nom personnalisé de la courbe de tendance
            trendline.Name = trendlineName;
            
            // Affichage de l'équation sur le graphique
            trendline.DisplayEquation = true;
            
            // Affichage de la valeur R‑carré sur le graphique
            trendline.DisplayRSquared = true;
            
            // Définition de la couleur de la ligne de tendance
            trendline.Color = Color.Red;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


