---
title: "Series.LegendEntry"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Series-Eigenschaft. Gibt den Legendeintrag für diese Serie zurück"
type: docs
url: /de/net/aspose.cells.charts/series/legendentry/
---
## Series.LegendEntry property

Liefert den Legendeintrag für diese Serie.

```csharp
public LegendEntry LegendEntry { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyLegendEntryDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Erhalte die erste Serie
            Series series = chart.NSeries[0];

            // Demonstriere die Funktionalität von LegendEntry
            Console.WriteLine("LegendEntry.IsDeleted before: " + series.LegendEntry.IsDeleted);
            series.LegendEntry.IsDeleted = true;
            Console.WriteLine("LegendEntry.IsDeleted after setting to true: " + series.LegendEntry.IsDeleted);
            series.LegendEntry.IsDeleted = false;
            Console.WriteLine("LegendEntry.IsDeleted after setting to false: " + series.LegendEntry.IsDeleted);

            // Speichere die Arbeitsmappe
            workbook.Save("SeriesPropertyLegendEntryDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [LegendEntry](../../legendentry/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


