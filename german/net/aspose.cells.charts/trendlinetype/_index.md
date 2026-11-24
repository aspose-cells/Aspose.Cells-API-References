---
title: "Enum TrendlineType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.TrendlineType enum. Stellt den Trendlinien-Typ dar"
type: docs
url: /de/net/aspose.cells.charts/trendlinetype/
---
## TrendlineType enumeration

Stellt den Trendlinien‑Typ dar.

```csharp
public enum TrendlineType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Exponential | `0` | Exponential |
| Linear | `1` | Linear |
| Logarithmic | `2` | Logarithmisch |
| MovingAverage | `3` | Gleitender Durchschnitt |
| Polynomial | `4` | Polynomial |
| Power | `5` | Potenz |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class TrendlineTypeDemo
    {
        public static void TrendlineTypeExample()
        {
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();
            
            // Ein neues Arbeitsblatt zum Excel-Objekt hinzufügen
            int sheetIndex = workbook.Worksheets.Add();
            
            // Abrufen der Referenz des neu hinzugefügten Arbeitsblatts durch Übergabe seines Blattindexes
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Hinzufügen von Beispielwerten zu Zellen
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Hinzufügen eines Diagramms zum Arbeitsblatt
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            
            // Zugriff auf die Instanz des neu hinzugefügten Diagramms
            Chart chart = worksheet.Charts[chartIndex];
            
            // Hinzufügen von NSeries (Diagrammdatenquelle) zum Diagramm vom Feld "A1" bis "B4"
            chart.NSeries.Add("A1:B4", true);
            
            // Festlegen der Datenquelle für die Kategoriedaten von NSeries
            chart.NSeries.CategoryData = "C1:C4";

            // Hinzufügen verschiedener Trendlinientypen zum Diagramm
            AddTrendline(chart, 0, TrendlineType.Linear, "Linear Trendline");
            AddTrendline(chart, 0, TrendlineType.Exponential, "Exponential Trendline");
            AddTrendline(chart, 0, TrendlineType.Logarithmic, "Logarithmic Trendline");
            AddTrendline(chart, 0, TrendlineType.MovingAverage, "Moving Average Trendline");
            AddTrendline(chart, 0, TrendlineType.Polynomial, "Polynomial Trendline");
            AddTrendline(chart, 0, TrendlineType.Power, "Power Trendline");

            // Die Excel-Datei speichern
            workbook.Save("TrendlineTypeExample.xlsx");
        }

        private static void AddTrendline(Chart chart, int seriesIndex, TrendlineType trendlineType, string trendlineName)
        {
            // Hinzufügen einer Trendlinie des angegebenen Typs zur angegebenen Serie
            int index = chart.NSeries[seriesIndex].TrendLines.Add(trendlineType);
            Trendline trendline = chart.NSeries[seriesIndex].TrendLines[index];
            
            // Festlegen des benutzerdefinierten Namens der Trendlinie
            trendline.Name = trendlineName;
            
            // Anzeige der Gleichung im Diagramm
            trendline.DisplayEquation = true;
            
            // Anzeige des R-Quadrat-Werts im Diagramm
            trendline.DisplayRSquared = true;
            
            // Festlegen der Farbe der Trendlinie
            trendline.Color = Color.Red;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


