---
title: "GradientStop.Position"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà GradientStop. La posizione della fermata"
type: docs
url: /it/net/aspose.cells.drawing/gradientstop/position/
---
## GradientStop.Position property

La posizione dello stop.

```csharp
public double Position { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);

            // Aggiungi un grafico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B3", true);

            // Configura il riempimento gradiente per la prima serie
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.Area.FillFormat.FillType = Aspose.Cells.Drawing.FillType.Gradient;
            series.Area.FillFormat.GradientFill.SetPresetThemeGradient(
                Aspose.Cells.Drawing.PresetThemeGradientType.RadialGradient, 
                ThemeColorType.Accent1);

            // Accedi e modifica le posizioni dei gradient stop
            GradientStopCollection stops = series.Area.FillFormat.GradientFill.GradientStops;
            stops[0].Position = 0;
            stops[1].Position = 50;
            stops[2].Position = 100;

            // Salva la cartella di lavoro
            workbook.Save("GradientStopPositionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [GradientStop](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


