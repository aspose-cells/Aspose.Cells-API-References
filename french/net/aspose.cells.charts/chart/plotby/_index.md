---
title: "Chart.PlotBy"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Chart. Obtient et définit si le tracé est par ligne ou par colonne"
type: docs
url: /fr/net/aspose.cells.charts/chart/plotby/
---
## Chart.PlotBy property

Obtient et définit si le tracé se fait par ligne ou par colonne.

```csharp
public PlotDataByType PlotBy { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPlotByDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["C1"].PutValue("Series 2");
            worksheet.Cells["C2"].PutValue(15);
            worksheet.Cells["C3"].PutValue(25);
            worksheet.Cells["C4"].PutValue(35);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Définir la source de données du graphique
            chart.SetChartDataRange("A1:C4", true);

            // Démontrer la propriété PlotBy
            Console.WriteLine("Default PlotBy: " + chart.PlotBy);
            
            // Créer un nouveau graphique avec un réglage différent de plot by
            int newChartIndex = worksheet.Charts.Add(ChartType.Column, 25, 0, 40, 8);
            Aspose.Cells.Charts.Chart newChart = worksheet.Charts[newChartIndex];
            newChart.SetChartDataRange("A1:C4", false); // Plot by row
            Console.WriteLine("New chart PlotBy: " + newChart.PlotBy);

            // Enregistrez le classeur
            workbook.Save("ChartPropertyPlotByDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* enum [PlotDataByType](../../plotdatabytype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


