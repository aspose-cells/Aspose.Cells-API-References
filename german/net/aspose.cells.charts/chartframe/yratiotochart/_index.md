---
title: "ChartFrame.YRatioToChart"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartFrame-Eigenschaft. Gibt die y-Koordinate der oberen linken Ecke in Einheiten des Verhältnisses des Diagrammbereichs zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells.charts/chartframe/yratiotochart/
---
## ChartFrame.YRatioToChart property

Liest oder legt fest die y‑Koordinate der oberen linken Ecke in Einheiten des Verhältnisses zum Diagrammbereich.

```csharp
public virtual double YRatioToChart { get; set; }
```

### Hinweise

Dies ist ein Bruchwert, sein gültiger Bereich liegt zwischen 0‑1. Wie konvertiert man Verhältnis‑Einheiten in Pixel? `YPixel = YRatioToChart * Chart.ChartObject.Height;`

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyYRatioToChartDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Greifen Sie auf den Diagrammtitel zu, der von ChartFrame erbt
            chart.Title.Text = "Sample Chart";
            
            // Aktuellen YRatioToChart-Wert anzeigen
            Console.WriteLine("Current Title YRatioToChart value: " + chart.Title.YRatioToChart);
            
            // Ändern Sie die Y‑Position des Titels relativ zum Diagrammbereich
            chart.Title.YRatioToChart = 0.1; // 10% from top of chart area
            
            // Neuen YRatioToChart‑Wert anzeigen
            Console.WriteLine("New Title YRatioToChart value: " + chart.Title.YRatioToChart);
            
            // Greifen Sie auf die Legende zu, die ebenfalls von ChartFrame erbt
            chart.Legend.Position = LegendPositionType.Top;
            
            // Aktuellen YRatioToChart‑Wert für die Legende anzeigen
            Console.WriteLine("Current Legend YRatioToChart value: " + chart.Legend.YRatioToChart);
            
            // Ändern Sie die Y‑Position der Legende relativ zum Diagrammbereich
            chart.Legend.YRatioToChart = 0.15; // 15% from top of chart area
            
            // Neuen YRatioToChart‑Wert für die Legende anzeigen
            Console.WriteLine("New Legend YRatioToChart value: " + chart.Legend.YRatioToChart);
            
            // Speichere die Arbeitsmappe
            workbook.Save("ChartFramePropertyYRatioToChartDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


