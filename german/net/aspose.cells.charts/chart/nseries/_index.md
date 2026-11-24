---
title: "Chart.NSeries"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Chart-Eigenschaft. Gibt eine SeriesCollection‑Sammlung zurück, die die Datenreihen im Diagramm darstellt"
type: docs
url: /de/net/aspose.cells.charts/chart/nseries/
---
## Chart.NSeries property

Gibt eine [`SeriesCollection`](../../seriescollection/)‑Sammlung zurück, die die Datenreihen im Diagramm darstellt.

```csharp
public SeriesCollection NSeries { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyNSeriesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Füge Beispieldaten zu Zellen hinzu
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue("Cat " + (i - 1));
                sheet.Cells["B" + i].PutValue(i * 10);
            }

            // Füge ein Diagramm hinzu
            int chartIndex = sheet.Charts.Add(ChartType.LineWithDataMarkers, 5, 2, 25, 11);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];

            // Legen Sie die Datenquelle für die Diagrammreihen mithilfe von NSeries fest
            chart.NSeries.Add("=Sheet1!$A$2:$B$10", true);

            // Diagrammtitel festlegen
            chart.Title.Text = "NSeries Demo Chart";

            // Speichere die Arbeitsmappe
            workbook.Save("NSeriesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SeriesCollection](../../seriescollection/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


