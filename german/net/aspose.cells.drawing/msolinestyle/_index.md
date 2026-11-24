---
title: "Enum MsoLineStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.MsoLineStyle-Enum. Stellt den Stil von Zeichenlinien dar"
type: docs
url: /de/net/aspose.cells.drawing/msolinestyle/
---
## MsoLineStyle enumeration

Stellt den Stil von Zeichenlinien dar.

```csharp
public enum MsoLineStyle
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Single | `0` | Einzelne Linie (mit Breite lineWidth) |
| ThickBetweenThin | `1` | Drei Linien, dünn, dick, dünn |
| ThinThick | `2` | Doppelte Linien, eine dünn, eine dick |
| ThickThin | `3` | Doppelte Linien, eine dick, eine dünn |
| ThinThin | `4` | Doppelte Linien gleicher Breite |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineStyleDemo
    {
        public static void MsoLineStyleExample()
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

            // Greifen Sie auf die primäre Kategorienachse zu
            Axis categoryAxis = chart.CategoryAxis;

            // Setzen Sie den Linienstil für die primäre Kategorienachse
            Line axisLine = categoryAxis.AxisLine;
            axisLine.CompoundType = MsoLineStyle.ThickBetweenThin;
            axisLine.Color = Color.Blue;
            axisLine.WeightPt = 2.0;

            // Geben Sie den Linienstil aus
            Console.WriteLine("Axis Line Style: " + axisLine.CompoundType);
            Console.WriteLine("Axis Line Color: " + axisLine.Color);
            Console.WriteLine("Axis Line Weight: " + axisLine.WeightPt);

            // Speichere die Arbeitsmappe
            workbook.Save("MsoLineStyleExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


