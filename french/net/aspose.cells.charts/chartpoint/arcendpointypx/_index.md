---
title: "ChartPoint.ArcEndPointYPx"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartPoint. Obtient la coordonnée y du point final de la section du secteur après l'appel de la méthode Chart.Calculate. S'applique aux graphiques en secteurs et en anneaux"
type: docs
url: /fr/net/aspose.cells.charts/chartpoint/arcendpointypx/
---
## ChartPoint.ArcEndPointYPx property

Obtient la coordonnée y du point final de la section du secteur après l'appel de la méthode Chart.Calculate(). S'applique aux graphiques Pie et Doughnut.

```csharp
public float ArcEndPointYPx { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyArcEndPointYPxDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("C1");
            worksheet.Cells["A3"].PutValue("C2");
            worksheet.Cells["A4"].PutValue("C3");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(8000);
            worksheet.Cells["B3"].PutValue(12000);
            worksheet.Cells["B4"].PutValue(14000);

            // Ajouter un graphique en secteurs
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calculer le graphique pour obtenir les positions des formes
            chart.Calculate();

            // Obtenir le premier point du graphique
            ChartPoint point = chart.NSeries[0].Points[0];

            // Afficher la valeur actuelle de ArcEndPointYPx
            Console.WriteLine("Current ArcEndPointYPx value: " + point.ArcEndPointYPx);

            // Étant donné que ArcEndPointYPx est en lecture seule, nous ne pouvons que le lire
            // La ligne suivante provoquerait une erreur de compilation :
            // point.ArcEndPointYPx = 150.5f;

            // Démontrer comment cette propriété affecte le graphique en secteurs
            Console.WriteLine("Pie slice end point Y coordinate: " + point.ArcEndPointYPx + " pixels");

            // Enregistrez le classeur
            workbook.Save("ChartPointPropertyArcEndPointYPxDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


