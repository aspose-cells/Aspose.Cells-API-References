---
title: "ChartArea.WidthRatioToChart"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartArea. Obtient ou définit le décalage horizontal depuis la colonne du coin inférieur droit en unités du ratio de la zone du graphique"
type: docs
url: /fr/net/aspose.cells.charts/chartarea/widthratiotochart/
---
## ChartArea.WidthRatioToChart property

Obtient ou définit le décalage horizontal depuis la colonne du coin inférieur droit, en unités de proportion de la zone de graphique.

```csharp
public override double WidthRatioToChart { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartAreaPropertyWidthRatioToChartDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajouter un graphique en colonnes
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calculer le graphique
            chart.Calculate();

            // Démontrez la propriété WidthRatioToChart
            Console.WriteLine("Chart Area Width Ratio: " + chart.ChartArea.WidthRatioToChart);
            
            // Modifiez le ratio et montrez le changement
            chart.ChartArea.WidthRatioToChart = 0.8;
            Console.WriteLine("Modified Chart Area Width Ratio: " + chart.ChartArea.WidthRatioToChart);
        }
    }
}
```

### Voir aussi

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


