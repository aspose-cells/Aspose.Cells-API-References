---
title: "Enum TickLabelAlignmentType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.TickLabelAlignmentType enum. Stellt den Textausrichtungstyp für die Tick-Labels auf der Achse dar."
type: docs
url: /de/net/aspose.cells.charts/ticklabelalignmenttype/
---
## TickLabelAlignmentType enumeration

Stellt den Textausrichtungstyp für die Tick‑Beschriftungen auf der Achse dar.

```csharp
public enum TickLabelAlignmentType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Center | `0` | Gibt an, dass der Text zentriert ist. |
| Left | `1` | Gibt an, dass der Text linksbündig ist. |
| Right | `2` | Gibt an, dass der Text rechtsbündig ist.. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TickLabelAlignmentTypeDemo
    {
        public static void TickLabelAlignmentTypeExample()
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

            // Serie zum Diagramm hinzufügen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Zugriff auf die Tick-Labels der Kategorienachse
            TickLabels tickLabels = chart.CategoryAxis.TickLabels;

            // Legt den Ausrichtungstyp für die Tick-Labels fest
            tickLabels.AlignmentType = TickLabelAlignmentType.Center;

            // Speichere die Arbeitsmappe
            workbook.Save("TickLabelAlignmentTypeExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


