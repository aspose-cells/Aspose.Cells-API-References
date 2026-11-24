---
title: "Klasse Sparkline"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.Sparkline-Klasse. Ein Sparkline stellt ein winziges Diagramm oder eine Grafik in einer Arbeitsblattzelle dar, die eine visuelle Darstellung von Daten liefert"
type: docs
url: /de/net/aspose.cells.charts/sparkline/
---
## Sparkline class

Ein Sparkline stellt ein winziges Diagramm oder eine Grafik in einer Arbeitsblattzelle dar, die eine visuelle Darstellung von Daten liefert.

```csharp
public class Sparkline
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Column](../../aspose.cells.charts/sparkline/column/) { get; } | Gibt den Spaltenindex des Sparkline zurück. |
| [DataRange](../../aspose.cells.charts/sparkline/datarange/) { get; set; } | Stellt den Datenbereich des Sparkline dar. |
| [Row](../../aspose.cells.charts/sparkline/row/) { get; } | Gibt den Zeilenindex des Sparkline zurück. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [ToImage](../../aspose.cells.charts/sparkline/toimage/#toimage)(ImageOrPrintOptions) | Konvertiert ein Sparkline in ein Bild. |
| [ToImage](../../aspose.cells.charts/sparkline/toimage/#toimage_1)(Stream, ImageOrPrintOptions) | Konvertiert ein Sparkline in ein Bild. |
| [ToImage](../../aspose.cells.charts/sparkline/toimage/#toimage_2)(string, ImageOrPrintOptions) | Konvertiert ein Sparkline in ein Bild. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SparklineDemo
    {
        public static void SparklineExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt einige Daten hinzu
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Definiert den CellArea für die Sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Fügt der Arbeitsmappe eine Sparkline-Gruppe hinzu
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, sheet.Name + "!A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Füge ein Sparkline zur Gruppe hinzu
            idx = group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 5);
            Sparkline line = group.Sparklines[idx];

            // Ausgabe der Sparkline-Details
            Console.WriteLine("Sparkline data range: " + line.DataRange + ", row: " + line.Row + ", column: " + line.Column);

            // Speichere die Sparkline als Bild
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = Aspose.Cells.Drawing.ImageType.Png,
                HorizontalResolution = 300,
                VerticalResolution = 300
            };
            line.ToImage("output.png", options);

            // Speichere die Arbeitsmappe
            workbook.Save("SparklineExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


