---
title: "Chart.PlotBy"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Chart‑Eigenschaft. Gibt an und legt fest, ob nach Zeile oder Spalte geplottet wird"
type: docs
url: /de/net/aspose.cells.charts/chart/plotby/
---
## Chart.PlotBy property

Liest und setzt, ob nach Zeile oder Spalte geplottet wird.

```csharp
public PlotDataByType PlotBy { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPlotByDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["C1"].PutValue("Series 2");
            worksheet.Cells["C2"].PutValue(15);
            worksheet.Cells["C3"].PutValue(25);
            worksheet.Cells["C4"].PutValue(35);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenquelle festlegen
            chart.SetChartDataRange("A1:C4", true);

            // PlotBy‑Eigenschaft demonstrieren
            Console.WriteLine("Default PlotBy: " + chart.PlotBy);
            
            // Neues Diagramm mit anderer Plot‑By‑Einstellung erstellen
            int newChartIndex = worksheet.Charts.Add(ChartType.Column, 25, 0, 40, 8);
            Aspose.Cells.Charts.Chart newChart = worksheet.Charts[newChartIndex];
            newChart.SetChartDataRange("A1:C4", false); // Plot by row
            Console.WriteLine("New chart PlotBy: " + newChart.PlotBy);

            // Speichere die Arbeitsmappe
            workbook.Save("ChartPropertyPlotByDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* enum [PlotDataByType](../../plotdatabytype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


