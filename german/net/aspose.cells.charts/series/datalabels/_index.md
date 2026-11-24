---
title: "Series.DataLabels"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Series‑Eigenschaft. Stellt das DataLabels‑Objekt für die angegebene ASeries dar"
type: docs
url: /de/net/aspose.cells.charts/series/datalabels/
---
## Series.DataLabels property

Stellt das DataLabels-Objekt für die angegebene ASeries dar.

```csharp
public DataLabels DataLabels { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyDataLabelsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greifen Sie auf das erste Arbeitsblatt zu und fügen Sie Beispieldaten hinzu
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Cells["A1"].PutValue("Products");
            dataSheet.Cells["B1"].PutValue("Users");
            dataSheet.Cells["A2"].PutValue("Aspose.Cells");
            dataSheet.Cells["B2"].PutValue(10000);
            dataSheet.Cells["A3"].PutValue("Aspose.Slides");
            dataSheet.Cells["B3"].PutValue(8000);
            dataSheet.Cells["A4"].PutValue("Aspose.Words");
            dataSheet.Cells["B4"].PutValue(12000);

            // Füge ein Diagrammblatt hinzu und erstelle ein Kreisdiagramm
            Worksheet chartSheet = workbook.Worksheets[workbook.Worksheets.Add(SheetType.Chart)];
            Chart chart = chartSheet.Charts[chartSheet.Charts.Add(ChartType.Pie, 7, 0, 20, 6)];

            // Seriendaten hinzufügen und Datenbeschriftungen konfigurieren
            Series series = chart.NSeries[chart.NSeries.Add("=Sheet1!$B$2:$B$4", true)];
            series.XValues = "=Sheet1!$A$2:$A$4";
            
            // DataLabels-Eigenschaften konfigurieren
            series.DataLabels.ShowValue = true;
            series.DataLabels.ShowCategoryName = true;
            series.DataLabels.ShowPercentage = true;
            series.DataLabels.LinkedSource = null; // Explicitly set to null

            // Speichere die Arbeitsmappe
            workbook.Save("SeriesPropertyDataLabelsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [DataLabels](../../datalabels/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


