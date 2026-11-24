---
title: "Series.SeriesLines"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Series-Eigenschaft. Gibt ein SeriesLines-Objekt zurück, das die Serienlinien für ein gestapeltes Balken- oder Säulendiagramm darstellt. Gilt nur für gestapelte Balken- und Säulendiagramme."
type: docs
url: /de/net/aspose.cells.charts/series/serieslines/
---
## Series.SeriesLines property

Gibt ein SeriesLines-Objekt zurück, das die Serienlinien für ein gestapeltes Balken‑ oder Säulendiagramm darstellt. Gilt nur für gestapelte Balken‑ und Säulendiagramme.

```csharp
public Line SeriesLines { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SeriesPropertySeriesLinesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["A5"].PutValue(4);
            
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Diagramm erstellen
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Serie hinzufügen
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";
            
            // Serienlinien anpassen
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.SeriesLines.Color = Color.Red;
            series.SeriesLines.Weight = Aspose.Cells.Drawing.WeightType.SingleLine;
            
            // Speichere die Arbeitsmappe
            workbook.Save("SeriesLinesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Line](../../../aspose.cells.drawing/line/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


