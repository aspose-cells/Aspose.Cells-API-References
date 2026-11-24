---
title: "ChartArea.XRatioToChart"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartArea-Eigenschaft. Gibt den horizontalen Versatz von der oberen linken Spalten-Ecke als Verhältnis zum Diagrammbereich zurück oder legt ihn fest."
type: docs
url: /de/net/aspose.cells.charts/chartarea/xratiotochart/
---
## ChartArea.XRatioToChart property

Ermittelt oder legt den horizontalen Versatz von der oberen linken Eckspalte, als Verhältnis zum Diagrammbereich.

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

    public class ChartAreaPropertyXRatioToChartDemo
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

            // Den Diagrammbereich abrufen
            ChartArea chartArea = chart.ChartArea;

            // Zeigen Sie den aktuellen XRatioToChart-Wert an
            Console.WriteLine("Current XRatioToChart value: " + chartArea.XRatioToChart);

            // Ändern Sie den XRatioToChart-Wert, um den Diagrammbereich horizontal zu verschieben
            chartArea.XRatioToChart = 0.2; // 20% from the left of the chart container

            // Zeigen Sie den neuen XRatioToChart-Wert an
            Console.WriteLine("New XRatioToChart value: " + chartArea.XRatioToChart);

            // Speichere die Arbeitsmappe
            workbook.Save("ChartAreaXRatioToChartDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


