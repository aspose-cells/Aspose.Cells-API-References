---
title: "GradientStop.Position"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété GradientStop. La position de l'arrêt"
type: docs
url: /fr/net/aspose.cells.drawing/gradientstop/position/
---
## GradientStop.Position property

La position du stop.

```csharp
public double Position { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class GradientStopPropertyPositionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);

            // Ajoutez un graphique
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B3", true);

            // Configurer le remplissage en dégradé pour la première série
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.Area.FillFormat.FillType = Aspose.Cells.Drawing.FillType.Gradient;
            series.Area.FillFormat.GradientFill.SetPresetThemeGradient(
                Aspose.Cells.Drawing.PresetThemeGradientType.RadialGradient, 
                ThemeColorType.Accent1);

            // Accéder et modifier les positions des arrêts de dégradé
            GradientStopCollection stops = series.Area.FillFormat.GradientFill.GradientStops;
            stops[0].Position = 0;
            stops[1].Position = 50;
            stops[2].Position = 100;

            // Enregistrez le classeur
            workbook.Save("GradientStopPositionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [GradientStop](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


