---
title: "Series.IsColorVaried"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Series-Eigenschaft. Gibt an, ob die Farbe der Punkte variiert. Das Diagramm muss nur eine Series enthalten oder ein Kreisdiagramm sein."
type: docs
url: /de/net/aspose.cells.charts/series/iscolorvaried/
---
## Series.IsColorVaried property

Stellt dar, ob die Farbe der Punkte variiert. Das Diagramm muss nur eine Serie enthalten oder ein Kreisdiagramm sein.

```csharp
public bool IsColorVaried { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyIsColorVariedDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Setze die IsColorVaried-Eigenschaft für die erste Series
            chart.NSeries[0].IsColorVaried = true;

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");

            // Überprüfen Sie die Eigenschaft
            Console.WriteLine("IsColorVaried: " + chart.NSeries[0].IsColorVaried);
        }
    }
}
```

### Siehe auch

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


