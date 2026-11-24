---
title: "DataLabels.BackgroundMode"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataLabels-Eigenschaft. Gibt den Anzeigemodus des Hintergrunds zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells.charts/datalabels/backgroundmode/
---
## DataLabels.BackgroundMode property

Liest und setzt den Anzeigemodus des Hintergrunds

```csharp
public BackgroundMode BackgroundMode { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyBackgroundModeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(5);

            // Ein Diagramm erstellen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B3", true);

            // Datenbeschriftungen abrufen
            Aspose.Cells.Charts.DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowValue = true;

            // Demonstrieren Sie die BackgroundMode-Eigenschaft
            dataLabels.BackgroundMode = BackgroundMode.Automatic; // Automatic background
            Console.WriteLine("BackgroundMode set to Automatic");

            // Speichere die Arbeitsmappe
            workbook.Save("DataLabelsBackgroundModeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [BackgroundMode](../../backgroundmode/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


