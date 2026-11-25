---
title: "Chart.PlotBy"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Chart. Ottiene e imposta se il tracciamento è per riga o colonna"
type: docs
url: /it/net/aspose.cells.charts/chart/plotby/
---
## Chart.PlotBy property

Ottiene e imposta se tracciare per riga o per colonna.

```csharp
public PlotDataByType PlotBy { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
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

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Imposta la fonte dati del grafico
            chart.SetChartDataRange("A1:C4", true);

            // Dimostra la proprietà PlotBy
            Console.WriteLine("Default PlotBy: " + chart.PlotBy);
            
            // Crea un nuovo grafico con impostazione PlotBy diversa
            int newChartIndex = worksheet.Charts.Add(ChartType.Column, 25, 0, 40, 8);
            Aspose.Cells.Charts.Chart newChart = worksheet.Charts[newChartIndex];
            newChart.SetChartDataRange("A1:C4", false); // Plot by row
            Console.WriteLine("New chart PlotBy: " + newChart.PlotBy);

            // Salva la cartella di lavoro
            workbook.Save("ChartPropertyPlotByDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PlotDataByType](../../plotdatabytype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


