---
title: "Title.XRatioToChart"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Title property. Gibt die x-Koordinate der oberen linken Ecke in Einheiten des Bruchteils des Diagrammbereichs zurück oder legt sie fest. X in Pixeln  XRatioToChart  Chart.ChartObject.Width"
type: docs
url: /de/net/aspose.cells.charts/title/xratiotochart/
---
## Title.XRatioToChart property

Liest oder schreibt die X‑Koordinate der oberen linken Ecke als Bruchteil des Diagrammbereichs. X in Pixeln = XRatioToChart * Chart.ChartObject.Width;

```csharp
public override double XRatioToChart { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TitlePropertyXRatioToChartDemo
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

            // Datenquelle für das Diagramm festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Rufen Sie den Diagrammtitel ab
            chart.Title.Text = "Sample Chart Title";
            Title title = chart.Title;

            // Aktuellen XRatioToChart-Wert anzeigen
            Console.WriteLine("Current XRatioToChart value: " + title.XRatioToChart);

            // Ändern Sie den XRatioToChart-Wert, um den Titel horizontal zu verschieben
            title.XRatioToChart = 0.25; // 25% from the left of the chart area
            Console.WriteLine("New XRatioToChart value: " + title.XRatioToChart);

            // Speichere die Arbeitsmappe
            workbook.Save("TitlePropertyXRatioToChartDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


