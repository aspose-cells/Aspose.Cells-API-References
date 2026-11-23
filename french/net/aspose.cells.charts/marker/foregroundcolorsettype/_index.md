---
title: "Marker.ForegroundColorSetType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Marker. Obtient ou définit le type d'ensemble de couleur de premier plan du marqueur"
type: docs
url: /fr/net/aspose.cells.charts/marker/foregroundcolorsettype/
---
## Marker.ForegroundColorSetType property

Obtient ou définit le type de jeu de couleur de premier plan du marqueur.

```csharp
public FormattingType ForegroundColorSetType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class MarkerPropertyForegroundColorSetTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Ajouter un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ajouter une série
            chart.NSeries.Add("A1:B3", true);
            
            // Configurer le marqueur de série
            Series series = chart.NSeries[0];
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.ForegroundColorSetType = FormattingType.Automatic;
            series.Marker.ForegroundColor = System.Drawing.Color.Black;

            workbook.Save("MarkerForegroundColorSetTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [FormattingType](../../formattingtype/)
* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


