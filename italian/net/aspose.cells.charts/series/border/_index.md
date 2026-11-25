---
title: "Series.Border"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. Rappresenta il bordo di un oggetto Series"
type: docs
url: /it/net/aspose.cells.charts/series/border/
---
## Series.Border property

Rappresenta il bordo di un oggetto Series.

```csharp
public Line Border { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SeriesPropertyBorderDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Year");
            worksheet.Cells["A2"].PutValue("2020");
            worksheet.Cells["A3"].PutValue("2021");
            worksheet.Cells["A4"].PutValue("2022");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(5000);
            worksheet.Cells["B3"].PutValue(7000);
            worksheet.Cells["B4"].PutValue(9000);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Aggiungi dati della serie
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ottieni la prima serie
            Series series = chart.NSeries[0];
            series.Name = "Sales Data";

            // Personalizza le proprietà del bordo
            series.Border.Color = System.Drawing.Color.Blue;
            series.Border.Weight = WeightType.MediumLine;
            series.Border.DashType = MsoLineDashStyle.Solid;
            series.Border.IsVisible = true;

            // Salva la cartella di lavoro
            workbook.Save("SeriesBorderDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Line](../../../aspose.cells.drawing/line/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


