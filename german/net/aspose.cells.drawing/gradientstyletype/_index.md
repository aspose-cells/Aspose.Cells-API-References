---
title: "Enum GradientStyleType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.GradientStyleType enum. Stellt den Verlaufs-Schattierungsstil dar"
type: docs
url: /de/net/aspose.cells.drawing/gradientstyletype/
---
## GradientStyleType enumeration

Stellt den Schattierungsstil des Gradienten dar.

```csharp
public enum GradientStyleType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| DiagonalDown | `0` | Diagonaler Abwärts-Schattierungsstil |
| DiagonalUp | `1` | Diagonaler Aufwärts-Schattierungsstil |
| FromCenter | `2` | Schattierungsstil von der Mitte |
| FromCorner | `3` | Schattierungsstil von der Ecke |
| Horizontal | `4` | Horizontaler Schattierungsstil |
| Vertical | `5` | Vertikaler Schattierungsstil |
| Unknown | `6` | Unbekannter Schattierungsstil. Nur für den Schattierungsstil (der nicht zu einem Mitglied von GradientStyleType gehört) in der Vorlagendatei. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientStyleTypeDemo
    {
        public static void GradientStyleTypeExample()
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Lege den Datenbereich des Diagramms fest
            chart.SetChartDataRange("A1:B4", true);

            // Zugriff auf den Plotbereich des Diagramms
            PlotArea plotArea = chart.PlotArea;

            // Zugriff auf das Füllformat des Plotbereichs
            FillFormat fillFormat = plotArea.Area.FillFormat;

            // Setze eine zweifarbige Farbverlauffüllung mit dem DiagonalDown-Stil
            fillFormat.SetTwoColorGradient(Color.Blue, Color.White, GradientStyleType.DiagonalDown, 1);

            // Gib den verwendeten Farbverlaufstil aus
            Console.WriteLine("Gradient Style: " + fillFormat.GradientStyle);

            // Speichere die Arbeitsmappe
            workbook.Save("GradientStyleTypeExample.xlsx");
            workbook.Save("GradientStyleTypeExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


