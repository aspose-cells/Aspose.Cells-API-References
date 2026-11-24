---
title: "Enum PrintSizeType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.PrintSizeType enum. Stellt die Größe des gedruckten Diagramms dar"
type: docs
url: /de/net/aspose.cells/printsizetype/
---
## PrintSizeType enumeration

Stellt die Größe des gedruckten Diagramms dar.

```csharp
public enum PrintSizeType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Full | `0` | Vollständige Seite verwenden. |
| Fit | `1` | Skalieren, um auf die Seite zu passen. |
| Custom | `2` | Benutzerdefiniert. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PrintSizeTypeDemo
    {
        public static void PrintSizeTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            // Hole das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells[0, 0].PutValue("Category");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue("A");
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue("B");
            worksheet.Cells[2, 1].PutValue(20);
            worksheet.Cells[3, 0].PutValue("C");
            worksheet.Cells[3, 1].PutValue(30);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Lege den Datenbereich für das Diagramm fest
            chart.SetChartDataRange("A1:B4", true);

            // Diagrammtitel festlegen
            chart.Title.Text = "Sample Chart";

            // Druckgröße des Diagramms festlegen
            chart.PrintSize = PrintSizeType.Fit;

            // Speichere die Arbeitsmappe
            workbook.Save("PrintSizeTypeExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


