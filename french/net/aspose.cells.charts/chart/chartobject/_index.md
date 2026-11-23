---
title: "Chart.ChartObject"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Chart. Représente le chartShape"
type: docs
url: /fr/net/aspose.cells.charts/chart/chartobject/
---
## Chart.ChartObject property

Représente le chartShape ;

```csharp
public ChartShape ChartObject { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPropertyChartObjectDemo
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

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Démontrer les propriétés de ChartObject
            chart.ChartObject.Placement = PlacementType.Move;
            chart.ChartObject.X = 100;
            chart.ChartObject.Y = 200;
            chart.ChartObject.Width = 400;
            chart.ChartObject.Height = 300;

            // Enregistrez le classeur
            workbook.Save("ChartObjectDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [ChartShape](../../../aspose.cells.drawing/chartshape/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


