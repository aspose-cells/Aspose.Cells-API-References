---
title: "SeriesLayoutProperties.ShowInnerPoints"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SeriesLayoutProperties. Indica se mostrare i punti dati nonoutlier"
type: docs
url: /it/net/aspose.cells.charts/serieslayoutproperties/showinnerpoints/
---
## SeriesLayoutProperties.ShowInnerPoints property

Indica se mostrare i punti dati non outlier.

```csharp
public bool ShowInnerPoints { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico a scatola e baffi
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

            // Aggiungi un grafico a scatola e baffi
            int chartIndex = worksheet.Charts.Add(ChartType.BoxWhisker, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Aggiungi serie al grafico
            chart.NSeries.Add("A2:A11", true);
            Series series = chart.NSeries[0];

            // Imposta le proprietà del layout della serie
            SeriesLayoutProperties layout = series.LayoutProperties;
            layout.ShowInnerPoints = true; // Demonstrate ShowInnerPoints property
            layout.ShowOutlierPoints = true;
            layout.ShowMeanMarker = true;

            // Calcola il grafico
            chart.Calculate();

            // Salva la cartella di lavoro
            workbook.Save("BoxWhiskerChart_ShowInnerPoints.xlsx");
        }
    }
}
```

### Vedi anche

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


