---
title: "ChartArea.YRatioToChart"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartArea-Eigenschaft. Liest oder liest den vertikalen Versatz von seiner oberen linken Zeilen­ecke in Einheiten des Verhältnisses zum Diagrammbereich"
type: docs
url: /de/net/aspose.cells.charts/chartarea/yratiotochart/
---
## ChartArea.YRatioToChart property

Ermittelt oder ermittelt den vertikalen Versatz von seiner oberen linken Eckzeile, in Einheiten des Verhältnisses zum Diagrammbereich.

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

    public class ChartAreaPropertyYRatioToChartDemo
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
            
            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Greifen Sie auf den Diagrammbereich zu
            ChartArea chartArea = chart.ChartArea;

            // Zeige den aktuellen YRatioToChart‑Wert an
            Console.WriteLine("Current YRatioToChart value: " + chartArea.YRatioToChart);

            // Ändere die YRatioToChart‑Eigenschaft (0,0 bis 1,0 entspricht 0 % bis 100 % des Diagrammbereichs)
            chartArea.YRatioToChart = 0.2; // Move chart area down by 20% of chart height

            // Zeige den neuen YRatioToChart‑Wert an
            Console.WriteLine("New YRatioToChart value: " + chartArea.YRatioToChart);

            // Speichern Sie die Arbeitsmappe, um den Effekt zu sehen
            workbook.Save("ChartAreaPropertyYRatioToChartDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


