---
title: "Enum TextAlignmentType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.TextAlignmentType-Enum. Enumeriert Textausrichtungstypen"
type: docs
url: /de/net/aspose.cells/textalignmenttype/
---
## TextAlignmentType enumeration

Enumeriert Textausrichtungstypen.

```csharp
public enum TextAlignmentType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| General | `1792` | Stellt allgemeine Textausrichtung dar. |
| Bottom | `528` | Stellt untere Textausrichtung dar. |
| Center | `1802` | Stellt mittlere Textausrichtung dar. |
| CenterAcross | `1286` | Stellt zentrierte Textausrichtung über mehrere Zellen dar. |
| Distributed | `807` | Stellt verteilte Textausrichtung dar. |
| Fill | `1284` | Stellt ausgefüllte Textausrichtung dar. |
| Justify | `1821` | Stellt Blocksatz-Textausrichtung dar. |
| Left | `257` | Stellt die linke Textausrichtung dar. |
| Right | `259` | Stellt die rechte Textausrichtung dar. |
| Top | `512` | Stellt die obere Textausrichtung dar. |
| JustifiedLow | `832` | Richtet den Text mit einer angepassten Kashida-Länge für arabischen Text aus. |
| ThaiDistributed | `896` | Verteilt thailändischen Text speziell, da jedes Zeichen als Wort behandelt wird. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TextAlignmentTypeDemo
    {
        public static void TextAlignmentTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Doe");

            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["B3"].PutValue(90);
            worksheet.Cells["B4"].PutValue(78);

            // Füge einer Zelle einen Kommentar hinzu
            Comment comment = worksheet.Comments[worksheet.Comments.Add("A1")];
            comment.Note = "This is a comment.";
            comment.TextHorizontalAlignment = TextAlignmentType.Center;
            comment.TextVerticalAlignment = TextAlignmentType.Top;

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Lege den Datenbereich des Diagramms fest
            chart.SetChartDataRange("A1:B4", true);

            // Passe den Diagrammtitel an
            chart.Title.Text = "Scores Chart";
            chart.Title.TextHorizontalAlignment = TextAlignmentType.Center;
            chart.Title.TextVerticalAlignment = TextAlignmentType.Top;

            // Speichere die Arbeitsmappe
            workbook.Save("TextAlignmentTypeExample.xlsx");

            // Ergebnisse ausgeben
            Console.WriteLine("Workbook saved successfully with text alignment settings.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


