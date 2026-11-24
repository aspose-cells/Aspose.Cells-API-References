---
title: "Klasse AxisBins"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.AxisBins Klasse. Stellt Achsenbehälter dar"
type: docs
url: /de/net/aspose.cells.charts/axisbins/
---
## AxisBins class

Stellt Achsen-Bins dar.

```csharp
public class AxisBins
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Count](../../aspose.cells.charts/axisbins/count/) { get; set; } | Liest oder legt die Anzahl der Achsenbehälter fest |
| [IsAutomatic](../../aspose.cells.charts/axisbins/isautomatic/) { get; set; } | Gibt an, ob die Achsenbehälter automatisch sind. |
| [IsByCategory](../../aspose.cells.charts/axisbins/isbycategory/) { get; set; } | Gibt an, ob die Gruppierung von Daten nach Kategorie aktiviert ist. |
| [Overflow](../../aspose.cells.charts/axisbins/overflow/) { get; set; } | Liest oder legt den Überlauf der Achsenbehälter fest |
| [Underflow](../../aspose.cells.charts/axisbins/underflow/) { get; set; } | Liest oder legt den Unterlauf der Achsenbehälter fest |
| [Width](../../aspose.cells.charts/axisbins/width/) { get; set; } | Liest oder legt die Breite des Achsenbehälters fest. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [ResetOverflow](../../aspose.cells.charts/axisbins/resetoverflow/)() | (**Obsolete.**) Setzt den Überlauf zurück |
| [ResetUnderflow](../../aspose.cells.charts/axisbins/resetunderflow/)() | (**Obsolete.**) Setzt den Unterlauf zurück |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisBinsDemo
    {
        public static void AxisBinsExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            // Ein neues Arbeitsblatt hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Histogram, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Datenreihen zum Diagramm hinzufügen
            chart.NSeries.Add("A1:A5", true);

            // Zugriff auf die Werteachse
            Axis valueAxis = chart.ValueAxis;

            // Zugriff auf die Behälter der Werteachse
            AxisBins bins = valueAxis.Bins;

            // Eigenschaften für die Behälter festlegen
            bins.IsByCategory = false;
            bins.IsAutomatic = true;
            bins.Width = 10.0;
            bins.Count = 5;
            bins.Overflow = 60.0;
            bins.Underflow = 0.0;

            // Überlauf und Unterlauf zurücksetzen
            //bins.ResetOverflow();
            //bins.ResetUnderflow();

            // Speichere die Arbeitsmappe
            workbook.Save("AxisBinsExample.xlsx");
            workbook.Save("AxisBinsExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


