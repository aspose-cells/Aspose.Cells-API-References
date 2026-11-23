---
title: "SeriesLayoutProperties.ShowInnerPoints"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SeriesLayoutProperties. Indique s’il faut afficher les points de données non‑outlier"
type: docs
url: /fr/net/aspose.cells.charts/serieslayoutproperties/showinnerpoints/
---
## SeriesLayoutProperties.ShowInnerPoints property

Indique s'il faut afficher les points de données non aberrants.

```csharp
public bool ShowInnerPoints { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertyShowInnerPointsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le diagramme à moustaches
            worksheet.Cells["A1"].PutValue("Series 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(40);
            worksheet.Cells["A4"].PutValue(15);
            worksheet.Cells["A5"].PutValue(20);
            worksheet.Cells["A6"].PutValue(25);
            worksheet.Cells["A7"].PutValue(30);
            worksheet.Cells["A8"].PutValue(35);
            worksheet.Cells["A9"].PutValue(40);
            worksheet.Cells["A10"].PutValue(45);
            worksheet.Cells["A11"].PutValue(50);

            // Ajouter un diagramme à moustaches
            int chartIndex = worksheet.Charts.Add(ChartType.BoxWhisker, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ajouter des séries au graphique
            chart.NSeries.Add("A2:A11", true);
            Series series = chart.NSeries[0];

            // Définir les propriétés de mise en forme des séries
            SeriesLayoutProperties layout = series.LayoutProperties;
            layout.ShowInnerPoints = true; // Demonstrate ShowInnerPoints property
            layout.ShowOutlierPoints = true;
            layout.ShowMeanMarker = true;

            // Calculer le graphique
            chart.Calculate();

            // Enregistrez le classeur
            workbook.Save("BoxWhiskerChart_ShowInnerPoints.xlsx");
        }
    }
}
```

### Voir aussi

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


