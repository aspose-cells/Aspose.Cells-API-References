---
title: "Enum LabelPositionType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.LabelPositionType enum. Stellt den Positionstyp von Datenbeschriftungen dar"
type: docs
url: /de/net/aspose.cells.charts/labelpositiontype/
---
## LabelPositionType enumeration

Stellt den Positionstyp für Datenbeschriftungen dar.

```csharp
public enum LabelPositionType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Center | `0` | Gilt nur für Balken- und 2D/3D-Kreisdiagramme |
| InsideBase | `1` | Gilt nur für Balken- und 2D/3D-Kreisdiagramme |
| InsideEnd | `2` | Gilt nur für Balkendiagramme |
| OutsideEnd | `3` | Gilt nur für Balken- und 2D/3D-Kreisdiagramme |
| Above | `4` | Gilt nur für Liniendiagramme |
| Below | `5` | Gilt nur für Liniendiagramme |
| Left | `6` | Gilt nur für Liniendiagramme |
| Right | `7` | Gilt nur für Liniendiagramme |
| BestFit | `8` | Gilt nur für 2D/3D-Kreisdiagramme |
| Moved | `9` | Benutzer hat die Datenbeschriftungen verschoben. Dies dient nur dem Lesen des Diagramms aus der Vorlagendatei. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class LabelPositionTypeDemo
    {
        public static void LabelPositionTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Beispieldaten für das Diagramm hinzu
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

            // Füge die Datenreihe dem Diagramm hinzu
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Greife auf die Datenbeschriftungen der ersten Reihe zu
            DataLabels dataLabels = chart.NSeries[0].DataLabels;

            // Position der Datenbeschriftungen festlegen
            dataLabels.Position = LabelPositionType.InsideBase;

            // Zeige den Kategorienamen in den Datenbeschriftungen
            dataLabels.ShowCategoryName = true;

            // Zeige den Wert in den Datenbeschriftungen
            dataLabels.ShowValue = true;

            // Speichere die Arbeitsmappe
            workbook.Save("LabelPositionTypeExample.xlsx");
            workbook.Save("LabelPositionTypeExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


