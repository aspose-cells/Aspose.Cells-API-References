---
title: "Chart.Is3D"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Chart. Indique si le graphique est un graphique 3D"
type: docs
url: /fr/net/aspose.cells.charts/chart/is3d/
---
## Chart.Is3D property

Indique si le graphique est un graphique 3D.

```csharp
public bool Is3D { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPropertyIs3DDemo
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
            worksheet.Cells["A5"].PutValue("Q4");

            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["B3"].PutValue(1500);
            worksheet.Cells["B4"].PutValue(1800);
            worksheet.Cells["B5"].PutValue(2100);

            // Ajouter un graphique en colonnes
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 6, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données pour le graphique
            chart.SetChartDataRange("A1:B5", true);

            // Afficher la valeur actuelle de Is3D
            Console.WriteLine("Current Is3D value: " + chart.Is3D);

            // Créer une version 3D du graphique
            int chart3DIndex = worksheet.Charts.Add(ChartType.Column3D, 6, 12, 20, 22);
            Chart chart3D = worksheet.Charts[chart3DIndex];
            chart3D.SetChartDataRange("A1:B5", true);

            // Afficher la valeur Is3D du graphique 3D
            Console.WriteLine("3D Chart Is3D value: " + chart3D.Is3D);

            // Enregistrez le classeur
            workbook.Save("ChartPropertyIs3DDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


