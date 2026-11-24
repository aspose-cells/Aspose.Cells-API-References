---
title: "Enum BubbleSizeRepresents"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.BubbleSizeRepresents enum. Gibt an, was die Größe der Blase in einem Blasendiagramm darstellt"
type: docs
url: /de/net/aspose.cells.charts/bubblesizerepresents/
---
## BubbleSizeRepresents enumeration

Stellt dar, was die Bubble‑Größe in einem Blasendiagramm repräsentiert.

```csharp
public enum BubbleSizeRepresents
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| SizeIsArea | `0` | Stellt den Wert von [`BubbleSizes`](../series/bubblesizes/) dar, der die Fläche der Blase ist. |
| SizeIsWidth | `1` | Stellt den Wert von [`BubbleSizes`](../series/bubblesizes/) dar, der die Breite der Blase ist. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class BubbleSizeRepresentsDemo
    {
        public static void BubbleSizeRepresentsExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten für das Blasendiagramm hinzu
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["B2"].PutValue(3);
            worksheet.Cells["B3"].PutValue(4);
            worksheet.Cells["C1"].PutValue(5);
            worksheet.Cells["C2"].PutValue(10);
            worksheet.Cells["C3"].PutValue(15);

            // Füge ein Blasendiagramm zum Arbeitsblatt hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Bubble, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Serie zum Blasendiagramm hinzufügen
            int seriesIndex = chart.NSeries.Add("A1:C3", true);
            Series series = chart.NSeries[seriesIndex];

            // Setzen Sie die X‑Werte, Y‑Werte und Blasengrößen
            series.XValues = "A1:A3";
            series.Values = "B1:B3";
            series.BubbleSizes = "C1:C3";

            // Darstellung der Blasengröße festlegen
            series.SizeRepresents = BubbleSizeRepresents.SizeIsArea;

            // Speichere die Arbeitsmappe
            workbook.Save("BubbleSizeRepresentsExample.xlsx");
            workbook.Save("BubbleSizeRepresentsExample.pdf");

            // Darstellung der Blasengröße festlegen
            series.SizeRepresents = BubbleSizeRepresents.SizeIsWidth;

            // Speichere die Arbeitsmappe
            workbook.Save("BubbleSizeRepresentsExample2.xlsx");
            workbook.Save("BubbleSizeRepresentsExample2.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


