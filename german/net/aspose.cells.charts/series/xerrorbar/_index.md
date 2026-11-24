---
title: "Series.XErrorBar"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Series-Eigenschaft. Stellt die X-Richtung-Fehlerbalken der Serie dar"
type: docs
url: /de/net/aspose.cells.charts/series/xerrorbar/
---
## Series.XErrorBar property

Stellt den X‑Richtungs-Fehlerbalken der Serie dar.

```csharp
public ErrorBar XErrorBar { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyXErrorBarDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("X Values");
            worksheet.Cells["B1"].PutValue("Y Values");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Fügen Sie eine Serie mit den Daten hinzu
            SeriesCollection seriesCollection = chart.NSeries;
            seriesCollection.Add("B2:B4", true);
            Series series = seriesCollection[0];
            series.XValues = "A2:A4";

            // Konfigurieren Sie die XErrorBar-Eigenschaften
            series.XErrorBar.DisplayType = ErrorBarDisplayType.Plus;
            series.XErrorBar.Amount = 0.5;
            series.XErrorBar.Type = ErrorBarType.FixedValue;

            // Speichere die Arbeitsmappe
            workbook.Save("SeriesPropertyXErrorBarDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ErrorBar](../../errorbar/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


