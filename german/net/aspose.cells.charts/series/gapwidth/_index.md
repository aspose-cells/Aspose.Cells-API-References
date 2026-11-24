---
title: "Series.GapWidth"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Series-Eigenschaft. Gibt den Abstand zwischen Balken- oder Säulenclustern als Prozentsatz der Balken- oder Säulenbreite zurück oder legt ihn fest. Der Wert dieser Eigenschaft muss zwischen 0 und 500 liegen"
type: docs
url: /de/net/aspose.cells.charts/series/gapwidth/
---
## Series.GapWidth property

Gibt den Abstand zwischen Balken‑ oder Spalten‑Clustern zurück oder setzt ihn, als Prozentsatz der Balken‑ oder Spaltenbreite. Der Wert dieser Eigenschaft muss zwischen 0 und 500 liegen.

```csharp
public short GapWidth { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyGapWidthDemo
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

            // Ein Säulendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Legen Sie die Lückenbreite für die erste Serie fest
            chart.NSeries[0].GapWidth = 150;

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


