---
title: "Enum ChartLineFormattingType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.ChartLineFormattingType enum. Stellt den Linientyp einer Diagrammlinie dar."
type: docs
url: /de/net/aspose.cells.charts/chartlineformattingtype/
---
## ChartLineFormattingType enumeration

Stellt den Formattyp der Diagrammlinie dar.

```csharp
public enum ChartLineFormattingType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Automatic | `0` | Stellt den automatischen Formatierungstyp dar. |
| Solid | `1` | Stellt den festen Formatierungstyp dar. |
| None | `2` | Stellt den Formatierungstyp "keine" dar. |
| Gradient | `3` | Verlauf |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartLineFormattingTypeDemo
    {
        public static void ChartLineFormattingTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            
            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Serie zum Diagramm hinzufügen
            chart.NSeries.Add("A1:B3", true);
            
            // Legen Sie die Kategoriedaten fest
            chart.NSeries.CategoryData = "A1:A3";
            
            // Legen Sie verschiedene Linienformatierungstypen für die Serie fest
            chart.NSeries[0].SeriesLines.FormattingType = ChartLineFormattingType.Solid;
            chart.NSeries[0].SeriesLines.Color = Color.Red;
            
            // Fügen Sie eine weitere Serie mit unterschiedlicher Formatierung hinzu
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries[1].SeriesLines.FormattingType = ChartLineFormattingType.Gradient;
            chart.NSeries[1].SeriesLines.Color = Color.Blue;
            
            // Speichere die Arbeitsmappe
            workbook.Save("ChartLineFormattingTypeExample.xlsx");
            workbook.Save("ChartLineFormattingTypeExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


