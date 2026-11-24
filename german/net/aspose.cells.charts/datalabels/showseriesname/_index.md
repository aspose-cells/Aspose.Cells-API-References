---
title: "DataLabels.ShowSeriesName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataLabels-Eigenschaft. Gibt an, ob der Serienname in den Datenbeschriftungen eines Diagramms angezeigt wird. True, um den Seriennamen anzuzeigen. False, um ihn zu verbergen"
type: docs
url: /de/net/aspose.cells.charts/datalabels/showseriesname/
---
## DataLabels.ShowSeriesName property

Gibt an, ob der Serienname in den Datenlabels eines Diagramms angezeigt wird. True zeigt den Seriennamen an. False blendet ihn aus.

```csharp
public bool ShowSeriesName { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyShowSeriesNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Series 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["B1"].PutValue("Series 2");
            worksheet.Cells["B2"].PutValue(15);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(35);

            // Ein Säulendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("A1:A4", true);
            chart.NSeries.Add("B1:B4", true);

            // Datenbeschriftungen für die erste Serie aktivieren
            Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;

            // Aktivieren Sie die Anzeige des Seriennamens für die Datenbeschriftung eines bestimmten Punktes
            var points = series.Points;
            points[1].DataLabels.ShowSeriesName = true;

            // Diagramm berechnen
            chart.Calculate();

            // Speichere die Arbeitsmappe
            workbook.Save("DataLabelsShowSeriesNameDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


