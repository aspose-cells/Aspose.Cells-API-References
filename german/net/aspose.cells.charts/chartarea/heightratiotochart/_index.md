---
title: "ChartArea.HeightRatioToChart"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartArea-Eigenschaft. Liest oder setzt den vertikalen Versatz von seiner unteren rechten Zeilen­ecke in Einheiten des Verhältnisses zum Diagrammbereich"
type: docs
url: /de/net/aspose.cells.charts/chartarea/heightratiotochart/
---
## ChartArea.HeightRatioToChart property

Liest oder setzt den vertikalen Versatz von seiner unteren rechten Eckzeilenposition, als Verhältnis des Diagrammbereichs.

```csharp
public override double HeightRatioToChart { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartAreaPropertyHeightRatioToChartDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 15, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Greifen Sie auf den Diagrammbereich zu
            ChartArea chartArea = chart.ChartArea;

            // Zeige den aktuellen HeightRatioToChart‑Wert an
            Console.WriteLine("Current HeightRatioToChart value: " + chartArea.HeightRatioToChart);

            // Setze einen neuen Wert für HeightRatioToChart (0,5 = 50 % der Diagrammhöhe)
            chartArea.HeightRatioToChart = 0.5;
            Console.WriteLine("New HeightRatioToChart value: " + chartArea.HeightRatioToChart);

            // Setze einen neuen Wert für WidthRatioToChart, um die kombinierte Wirkung zu demonstrieren
            chartArea.WidthRatioToChart = 0.8;

            // Speichere die Arbeitsmappe, um die Änderungen zu sehen
            workbook.Save("ChartAreaPropertyHeightRatioToChartDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


