---
title: "Enum GradientDirectionType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.GradientDirectionType enum. Stellt alle Richtungsarten des Farbverlaufs dar"
type: docs
url: /de/net/aspose.cells.drawing/gradientdirectiontype/
---
## GradientDirectionType enumeration

Stellt alle Richtungsarten von Verläufen dar.

```csharp
public enum GradientDirectionType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| FromUpperLeftCorner | `0` | FromUpperLeftCorner |
| FromUpperRightCorner | `1` | FromUpperRightCorner |
| FromLowerLeftCorner | `2` | FromLowerLeftCorner |
| FromLowerRightCorner | `3` | FromLowerRightCorner |
| FromCenter | `4` | FromCenter |
| Unknown | `5` | Unbekannt |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientDirectionTypeDemo
    {
        public static void GradientDirectionTypeExample()
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

            // Setzen Sie eine zweifarbige Farbverlaufsfüllung mit einer bestimmten Richtung
            fillFormat.SetTwoColorGradient(Color.Blue, Color.LightBlue, GradientStyleType.DiagonalDown, 1);
            fillFormat.GradientFill.SetGradient(GradientFillType.Linear, 45, GradientDirectionType.FromUpperLeftCorner);

            // Geben Sie den Farbverlaufsrichtungstyp aus
            Console.WriteLine("Gradient Direction Type: " + fillFormat.GradientFill.DirectionType);

            // Speichere die Arbeitsmappe
            workbook.Save("GradientDirectionTypeExample.xlsx");
            workbook.Save("GradientDirectionTypeExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


