---
title: "ChartFrame.DefaultHeight"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartFrame-Eigenschaft. Gibt die Höhe der Standardposition in Einheiten von 1/4000 des Diagrammbereichs an"
type: docs
url: /de/net/aspose.cells.charts/chartframe/defaultheight/
---
## ChartFrame.DefaultHeight property

Gibt die Höhe der Standardposition in Einheiten von 1/4000 des Diagrammbereichs an.

```csharp
[Obsolete("Use ChartFrame.DefaultHeightRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int DefaultHeight { get; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die Eigenschaft ChartFrame.DefaultHeightRatioToChart. DefaultHeight = (int)(DefaultHeightRatioToChart * 4000); Diese Eigenschaft wird 12 Monate später, seit Februar 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erfahren haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultHeightDemo
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

            // Greifen Sie auf den Titel des Diagramms zu (der ein ChartFrame ist)
            ChartFrame chartTitle = chart.Title;
            
            // Zeigen Sie den aktuellen DefaultHeight-Wert an (schreibgeschützte Eigenschaft)
            Console.WriteLine("Current DefaultHeight value: " + chartTitle.DefaultHeight);

            // Demonstrieren Sie, wie DefaultHeight das Diagrammlayout beeinflusst
            Console.WriteLine("DefaultHeightRatioToChart: " + chartTitle.DefaultHeightRatioToChart);
            Console.WriteLine("Current HeightRatioToChart: " + chartTitle.HeightRatioToChart);

            // Passen Sie die Höhe mit der schreibbaren Eigenschaft an
            chartTitle.HeightRatioToChart = chartTitle.DefaultHeightRatioToChart * 1.5;
            Console.WriteLine("New HeightRatioToChart: " + chartTitle.HeightRatioToChart);

            // Ergebnis speichern
            workbook.Save("ChartFrameDefaultHeightDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


