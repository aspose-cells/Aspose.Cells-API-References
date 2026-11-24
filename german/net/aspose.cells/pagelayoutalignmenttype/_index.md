---
title: "Enum PageLayoutAlignmentType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.PageLayoutAlignmentType enum. Enumeriert die Ausrichtungsarten des Seitenlayouts"
type: docs
url: /de/net/aspose.cells/pagelayoutalignmenttype/
---
## PageLayoutAlignmentType enumeration

Enumeriert Seitengestaltungs-Ausrichtungstypen.

```csharp
public enum PageLayoutAlignmentType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Bottom | `0` | Stellt die untere Seitenlayout-Ausrichtung dar. |
| Center | `1` | Stellt die zentrale Seitenlayout-Ausrichtung dar. |
| Left | `2` | Stellt die linke Seitenlayout-Ausrichtung dar. |
| Right | `3` | Stellt die rechte Seitenlayout-Ausrichtung dar. |
| Top | `4` | Stellt die obere Seitenlayout-Ausrichtung dar. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PageLayoutAlignmentTypeDemo
    {
        public static void PageLayoutAlignmentTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Beispieldaten zum Arbeitsblatt hinzu
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(456);
            worksheet.Cells["A4"].PutValue(789);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Lege den Datenbereich für das Diagramm fest
            chart.SetChartDataRange("A1:A4", true);

            // Setze den Titel des Diagramms
            chart.Title.Text = "Sample Chart";

            // Speichere die Arbeitsmappe in einer Datei
            workbook.Save("PageLayoutAlignmentTypeExample.xlsx");

            // Exportiere das Diagramm als PDF mit spezifischer Seitenlayout-Ausrichtung
            chart.ToPdf("ChartExample.pdf", 8.5f, 11f, PageLayoutAlignmentType.Center, PageLayoutAlignmentType.Center);

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


