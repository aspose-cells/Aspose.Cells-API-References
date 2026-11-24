---
title: "Series.HiLoLines"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Series-Eigenschaft. Gibt ein HiLoLines-Objekt zurück, das die Hoch‑Tief‑Linien für eine Serie in einem Liniendiagramm darstellt. Gilt nur für Liniendiagramme"
type: docs
url: /de/net/aspose.cells.charts/series/hilolines/
---
## Series.HiLoLines property

Gibt ein HiLoLines-Objekt zurück, das die Hoch‑Tief‑Linien für eine Serie in einem Liniendiagramm darstellt. Gilt nur für Liniendiagramme.

```csharp
public Line HiLoLines { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class SeriesPropertyHiLoLinesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["A5"].PutValue("Q4");

            worksheet.Cells["B1"].PutValue("High");
            worksheet.Cells["B2"].PutValue(120);
            worksheet.Cells["B3"].PutValue(90);
            worksheet.Cells["B4"].PutValue(150);
            worksheet.Cells["B5"].PutValue(110);

            worksheet.Cells["C1"].PutValue("Low");
            worksheet.Cells["C2"].PutValue(80);
            worksheet.Cells["C3"].PutValue(60);
            worksheet.Cells["C4"].PutValue(100);
            worksheet.Cells["C5"].PutValue(70);

            // Ein Liniendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 6, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B1:B5", true);
            chart.NSeries.Add("C1:C5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // HiLoLines für die erste Serie aktivieren
            Series series = chart.NSeries[0];
            series.HasHiLoLines = true;

            // Zugriff auf und Ändern von HiLoLines-Eigenschaften
            Line hiLoLines = series.HiLoLines;
            Console.WriteLine("HiLoLines visibility: " + hiLoLines.IsVisible);

            // Aussehen von HiLoLines anpassen
            hiLoLines.Color = System.Drawing.Color.Red;
            hiLoLines.Weight = WeightType.MediumLine;
            hiLoLines.DashType = MsoLineDashStyle.DashDot;
            hiLoLines.IsVisible = true;

            // Ergebnis speichern
            workbook.Save("SeriesPropertyHiLoLinesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Line](../../../aspose.cells.drawing/line/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


