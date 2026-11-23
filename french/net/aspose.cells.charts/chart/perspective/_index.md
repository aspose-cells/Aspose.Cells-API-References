---
title: "Chart.Perspective"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Chart propriété. Retourne ou définit la perspective de la vue du graphique tridimensionnel. Doit être comprise entre 0 et 100. Cette propriété est ignorée si la propriété RightAngleAxes est vraie"
type: docs
url: /fr/net/aspose.cells.charts/chart/perspective/
---
## Chart.Perspective property

Renvoie ou définit la perspective de la vue du graphique tridimensionnel. Doit être comprise entre 0 et 100. Cette propriété est ignorée si la propriété RightAngleAxes est True.

```csharp
public short Perspective { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPerspectiveDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Ajouter un graphique à colonnes 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Définir les propriétés de perspective du graphique 3D
            chart.Perspective = 30; // Perspective angle (0-100)
            chart.RotationAngle = 15; // Rotation angle
            chart.Elevation = 20; // Elevation angle
            chart.RightAngleAxes = false; // Enable perspective projection
            chart.AutoScaling = true; // Auto scale the chart

            // Enregistrez le classeur
            workbook.Save("ChartPerspectiveDemo.xlsx");

            Console.WriteLine("Chart with perspective settings created successfully.");
        }
    }
}
```

### Voir aussi

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


