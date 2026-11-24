---
title: "ChartArea.Width"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartArea-Eigenschaft. Liest oder setzt den horizontalen Versatz von seiner unteren rechten Spalten­ecke in Einheiten von 1/4000 des Diagrammbereichs"
type: docs
url: /de/net/aspose.cells.charts/chartarea/width/
---
## ChartArea.Width property

Liest oder setzt den horizontalen Versatz von seiner unteren rechten Spalten­ecke, in Einheiten von 1/4000 des Diagrammbereichs.

```csharp
[Obsolete("Use ChartArea.WidthRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Width { get; set; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die ChartArea.WidthRatioToChart‑Eigenschaft. Width = WidthRatioToChart * 4000. Diese Eigenschaft wird 12 Monate später, seit Februar 2025, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartAreaPropertyWidthDemo
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

            // Den Diagrammbereich abrufen
            ChartArea chartArea = chart.ChartArea;

            // Setze und demonstriere die Width‑Eigenschaft
            Console.WriteLine("Original Width: " + chartArea.Width);
            chartArea.Width = 800; // Set new width
            Console.WriteLine("Modified Width: " + chartArea.Width);

            // Speichere die Arbeitsmappe
            workbook.Save("ChartAreaWidthDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


