---
title: "Series.Has3DEffect"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà della serie. True se la serie ha un aspetto tridimensionale"
type: docs
url: /it/net/aspose.cells.charts/series/has3deffect/
---
## Series.Has3DEffect property

Vero se la serie ha un aspetto tridimensionale.

```csharp
public bool Has3DEffect { get; set; }
```

### Osservazioni

Si applica solo ai grafici Bubble o Bubble3D.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyHas3DEffectDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Q3");

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Aggiungi serie
            int seriesIndex = chart.NSeries.Add("A1:B3", true);
            chart.NSeries.CategoryData = "C1:C3";
            
            // Ottieni la serie e imposta l'effetto 3D
            Series series = chart.NSeries[seriesIndex];
            series.Has3DEffect = true;
            series.Bar3DShapeType = Bar3DShapeType.Cylinder;

            // Salva la cartella di lavoro
            workbook.Save("Series3DEffectDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


