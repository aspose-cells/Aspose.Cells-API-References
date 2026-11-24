---
title: "ChartFrame.DefaultY"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartFrame-Eigenschaft. Stellt das y der Standardposition in Einheiten von 1/4000 der Diagrammfläche dar."
type: docs
url: /de/net/aspose.cells.charts/chartframe/defaulty/
---
## ChartFrame.DefaultY property

Stellt das y der Standardposition in Einheiten von 1/4000 der Diagrammfläche dar.

```csharp
[Obsolete("Use ChartFrame.DefaultYRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int DefaultY { get; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die ChartFrame.DefaultYRatioToChart‑Eigenschaft. DefaultY = (int)(DefaultYRatioToChart * 4000); Diese Eigenschaft wird 12 Monate später, seit Februar 2025, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultYDemo
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
            
            // Greifen Sie auf den Diagrammtitel zu, der von ChartFrame erbt
            chart.Title.Text = "Sample Chart";
            ChartFrame chartFrame = chart.Title;
            
            // Den aktuellen DefaultY‑Wert anzeigen (schreibgeschützte Eigenschaft)
            Console.WriteLine("DefaultY value (1/4000 of chart area): " + chartFrame.DefaultY);
            Console.WriteLine("DefaultY ratio to chart area: " + chartFrame.DefaultYRatioToChart);
            
            // Demonstrieren, wie DefaultY die Positionierung beeinflusst, indem es mit der aktuellen Position verglichen wird
            Console.WriteLine("Current Y position (ratio): " + chartFrame.YRatioToChart);
            
            // Position mit SetPositionAuto() auf Standard zurücksetzen
            chartFrame.SetPositionAuto();
            Console.WriteLine("Y position after reset (ratio): " + chartFrame.YRatioToChart);
            
            // Ergebnis speichern
            workbook.Save("ChartFramePropertyDefaultYDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


