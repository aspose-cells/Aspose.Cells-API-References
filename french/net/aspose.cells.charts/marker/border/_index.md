---
title: "Marker.Border"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Marker. Obtient la bordure"
type: docs
url: /fr/net/aspose.cells.charts/marker/border/
---
## Marker.Border property

Obtient le [`border`](../../../aspose.cells.drawing/line/).

```csharp
public Line Border { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MarkerPropertyBorderDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue(3);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B4"].PutValue(6);

            // Créer un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.ScatterConnectedByLinesWithoutDataMarker, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Configurer les séries - corriger l'erreur de conversion en récupérant les séries depuis la collection
            int seriesIndex = chart.NSeries.Add("B2:B4", true);
            Series series = chart.NSeries[seriesIndex];
            series.XValues = "A2:A4";
            
            // Personnaliser la bordure du marqueur
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.MarkerSize = 10;
            series.Marker.Area.ForegroundColor = Color.LightBlue;
            series.Marker.Border.FormattingType = ChartLineFormattingType.Solid;
            series.Marker.Border.Color = Color.DarkBlue;
            series.Marker.Border.Weight = WeightType.MediumLine;

            workbook.Save("MarkerBorderDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* class [Line](../../../aspose.cells.drawing/line/)
* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


