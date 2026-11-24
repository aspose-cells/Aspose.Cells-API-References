---
title: "Chart.SeriesAxis"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Diagramm-Eigenschaft. Gibt die Serienachse des Diagramms zurück"
type: docs
url: /de/net/aspose.cells.charts/chart/seriesaxis/
---
## Chart.SeriesAxis property

Liest die Reihen‑Achse des Diagramms.

```csharp
public Axis SeriesAxis { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertySeriesAxisDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Series");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Product A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["C1"].PutValue("Product B");
            worksheet.Cells["C2"].PutValue(150);
            worksheet.Cells["C3"].PutValue(250);
            worksheet.Cells["C4"].PutValue(350);

            // Fügen Sie ein 3D gruppiertes Säulendiagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column3DClustered, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B1:C4", true);

            // Zugriff auf die SeriesAxis und Konfiguration
            Axis seriesAxis = chart.SeriesAxis;
            seriesAxis.Title.Text = "Product Series";
            seriesAxis.Title.Font.Size = 12;
            seriesAxis.Title.Font.IsBold = true;
            seriesAxis.MajorTickMark = TickMarkType.Cross;
            seriesAxis.MinorTickMark = TickMarkType.Outside;

            // Speichere die Arbeitsmappe
            workbook.Save("ChartPropertySeriesAxisDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Axis](../../axis/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


