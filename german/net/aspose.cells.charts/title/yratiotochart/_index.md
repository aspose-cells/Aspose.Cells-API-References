---
title: "Title.YRatioToChart"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Title property. Gibt die y-Koordinate der oberen linken Ecke in Einheiten des Bruchteils des Diagrammbereichs zurück oder legt sie fest. Y in Pixeln  YRatioToChart  Chart.ChartObject.Width"
type: docs
url: /de/net/aspose.cells.charts/title/yratiotochart/
---
## Title.YRatioToChart property

Liest oder schreibt die Y‑Koordinate der oberen linken Ecke als Bruchteil des Diagrammbereichs. Y in Pixeln = YRatioToChart * Chart.ChartObject.Width;

```csharp
public override double YRatioToChart { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TitlePropertyYRatioToChartDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Rufen Sie den Diagrammtitel ab
            chart.Title.Text = "Sample Chart Title";
            Title chartTitle = chart.Title;

            // Aktuellen YRatioToChart-Wert anzeigen
            Console.WriteLine("Current YRatioToChart value: " + chartTitle.YRatioToChart);

            // Ändern Sie die YRatioToChart-Eigenschaft, um den Titel vertikal zu verschieben
            chartTitle.YRatioToChart = 0.1; // 10% from the top of the chart area
            Console.WriteLine("New YRatioToChart value: " + chartTitle.YRatioToChart);

            // Speichere die Arbeitsmappe
            workbook.Save("TitlePropertyYRatioToChartDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


