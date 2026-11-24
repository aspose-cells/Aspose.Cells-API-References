---
title: "Enum MsoArrowheadLength"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.MsoArrowheadLength enum. Enumeriert die Linienendbreite der Formrandlinie"
type: docs
url: /de/net/aspose.cells.drawing/msoarrowheadlength/
---
## MsoArrowheadLength enumeration

Enumeriert die Endbreite der Linien des Formrahmens.

```csharp
public enum MsoArrowheadLength
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Short | `0` | Kurze Linienendlänge |
| Medium | `1` | Mittlere Linienendlänge |
| Long | `2` | Lange Linienendlänge |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoArrowheadLengthDemo
    {
        public static void MsoArrowheadLengthExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Lege den Datenbereich des Diagramms fest
            chart.SetChartDataRange("A1:B4", true);

            // Erstellen Sie eine Linienform für das Diagramm
            Line line = chart.Line;

            // Setze die Pfeilspitzenlängen
            line.BeginArrowLength = MsoArrowheadLength.Medium;
            line.EndArrowLength = MsoArrowheadLength.Long;

            // Gib die Pfeilspitzenlängen aus
            Console.WriteLine("Begin Arrowhead Length: " + line.BeginArrowLength);
            Console.WriteLine("End Arrowhead Length: " + line.EndArrowLength);

            // Speichere die Arbeitsmappe
            workbook.Save("MsoArrowheadLengthExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


