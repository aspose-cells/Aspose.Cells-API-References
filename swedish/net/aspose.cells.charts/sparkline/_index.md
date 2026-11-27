---
title: "Klass Sparkline"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.Sparkline klass. En sparkline representerar ett litet diagram eller grafik i en kalkylbladscell som ger en visuell representation av data"
type: docs
url: /sv/net/aspose.cells.charts/sparkline/
---
## Sparkline class

En sparkline representerar ett litet diagram eller grafik i en kalkylbladscell som ger en visuell representation av data.

```csharp
public class Sparkline
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Column](../../aspose.cells.charts/sparkline/column/) { get; } | Hämtar kolumnindexet för sparkline-objektet. |
| [DataRange](../../aspose.cells.charts/sparkline/datarange/) { get; set; } | Representerar dataintervallet för sparkline-objektet. |
| [Row](../../aspose.cells.charts/sparkline/row/) { get; } | Hämtar radindex för sparkline. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [ToImage](../../aspose.cells.charts/sparkline/toimage/#toimage)(ImageOrPrintOptions) | Konverterar en sparkline till en bild. |
| [ToImage](../../aspose.cells.charts/sparkline/toimage/#toimage_1)(Stream, ImageOrPrintOptions) | Konverterar en sparkline till en bild. |
| [ToImage](../../aspose.cells.charts/sparkline/toimage/#toimage_2)(string, ImageOrPrintOptions) | Konverterar en sparkline till en bild. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till lite data i kalkylbladet
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Definiera CellArea för sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Lägg till en sparkline‑grupp i kalkylbladet
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, sheet.Name + "!A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Lägg till en sparkline i gruppen
            idx = group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 5);
            Sparkline line = group.Sparklines[idx];

            // Skriv ut sparkline-detaljer
            Console.WriteLine("Sparkline data range: " + line.DataRange + ", row: " + line.Row + ", column: " + line.Column);

            // Spara sparkline som en bild
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = Aspose.Cells.Drawing.ImageType.Png,
                HorizontalResolution = 300,
                VerticalResolution = 300
            };
            line.ToImage("output.png", options);

            // Spara arbetsboken
            workbook.Save("SparklineExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


