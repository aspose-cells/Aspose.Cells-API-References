---
title: "Series.SizeRepresents"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Series-Eigenschaft. Gibt an, was die Blasengröße in einem Blasendiagramm darstellt, oder legt fest"
type: docs
url: /de/net/aspose.cells.charts/series/sizerepresents/
---
## Series.SizeRepresents property

Liest oder setzt, was die Blasengröße in einem Blasendiagramm darstellt.

```csharp
public BubbleSizeRepresents SizeRepresents { get; set; }
```

### Hinweise

BubbleSizeRepresents.SizeIsArea bedeutet, dass der Wert [`BubbleSizes`](../bubblesizes/) die Fläche der Blase ist. BubbleSizeRepresents.SizeIsWidth bedeutet, dass der Wert [`BubbleSizes`](../bubblesizes/) die Breite der Blase ist.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertySizeRepresentsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Beispieldaten für Blasendiagramm hinzufügen
            sheet.Cells["A1"].PutValue("X");
            sheet.Cells["B1"].PutValue("Y");
            sheet.Cells["C1"].PutValue("Size");
            for (int i = 2; i <= 5; i++)
            {
                sheet.Cells["A" + i].PutValue(i);
                sheet.Cells["B" + i].PutValue(i * 2);
                sheet.Cells["C" + i].PutValue(i * 0.5);
            }

            // Ein Blasendiagramm hinzufügen
            int chartIndex = sheet.Charts.Add(ChartType.Bubble, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // Seriendaten festlegen
            SeriesCollection series = chart.NSeries;
            series.Add("B2:B5", true);
            series.CategoryData = "A2:A5";
            series[0].BubbleSizes = "C2:C5";

            // SizeRepresents‑Eigenschaft festlegen
            series[0].SizeRepresents = BubbleSizeRepresents.SizeIsArea;

            // Speichere die Arbeitsmappe
            workbook.Save("SeriesPropertySizeRepresentsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [BubbleSizeRepresents](../../bubblesizerepresents/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


