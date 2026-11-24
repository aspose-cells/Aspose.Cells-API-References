---
title: "Enum TimeUnit"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.TimeUnit Enum. Stellt die Basiseinheit für die Kategorienachse dar."
type: docs
url: /de/net/aspose.cells.charts/timeunit/
---
## TimeUnit enumeration

Stellt die Basiseinheit für die Kategorienachse dar.

```csharp
public enum TimeUnit
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Days | `0` | Tage |
| Months | `1` | Monate |
| Years | `2` | Jahre |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TimeUnitDemo
    {
        public static void TimeUnitExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            // Ein neues Arbeitsblatt hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 2, 1));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["B1"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["B3"].PutValue(300);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Serie zum Diagramm hinzufügen
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Stellen Sie die Kategorienachse so ein, dass Zeiteinheiten verwendet werden
            Axis categoryAxis = chart.CategoryAxis;
            categoryAxis.CategoryType = CategoryType.TimeScale;
            categoryAxis.BaseUnitScale = TimeUnit.Months;
            categoryAxis.MajorUnitScale = TimeUnit.Months;
            categoryAxis.MinorUnitScale = TimeUnit.Days;

            // Passen Sie das Aussehen des Diagramms an
            chart.Title.Text = "Sample Chart with Time Units";
            chart.ValueAxis.Title.Text = "Values";
            chart.CategoryAxis.Title.Text = "Dates";

            // Speichere die Arbeitsmappe
            workbook.Save("TimeUnitExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


