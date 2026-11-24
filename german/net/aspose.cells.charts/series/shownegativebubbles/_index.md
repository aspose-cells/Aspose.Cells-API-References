---
title: "Series.ShowNegativeBubbles"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Series‑Eigenschaft. Wahr, wenn negative Blasen für die Diagrammgruppe angezeigt werden. Nur für Blasendiagramme gültig."
type: docs
url: /de/net/aspose.cells.charts/series/shownegativebubbles/
---
## Series.ShowNegativeBubbles property

Wahr, wenn negative Blasen für die Diagrammgruppe angezeigt werden. Gültig nur für Blasendiagramme.

```csharp
public bool ShowNegativeBubbles { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyShowNegativeBubblesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für Blasendiagramm hinzufügen
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["B2"].PutValue(2);
            worksheet.Cells["B3"].PutValue(-3);
            worksheet.Cells["B4"].PutValue(4);
            
            worksheet.Cells["C1"].PutValue("Size");
            worksheet.Cells["C2"].PutValue(5);
            worksheet.Cells["C3"].PutValue(6);
            worksheet.Cells["C4"].PutValue(7);

            // Ein Blasendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Bubble, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            SeriesCollection seriesCollection = chart.NSeries;
            seriesCollection.Add("B2:B4", true);
            seriesCollection.CategoryData = "A2:A4";
            seriesCollection[0].BubbleSizes = "C2:C4";

            // Greife auf die erste Serie zu und setze die ShowNegativeBubbles‑Eigenschaft
            Series series = chart.NSeries[0];
            series.ShowNegativeBubbles = true;

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


