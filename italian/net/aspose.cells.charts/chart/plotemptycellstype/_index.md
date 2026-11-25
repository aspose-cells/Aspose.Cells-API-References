---
title: "Chart.PlotEmptyCellsType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Chart. Ottiene e imposta come tracciare le celle vuote"
type: docs
url: /it/net/aspose.cells.charts/chart/plotemptycellstype/
---
## Chart.PlotEmptyCellsType property

Ottiene e imposta come tracciare le celle vuote.

```csharp
public PlotEmptyCellsType PlotEmptyCellsType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPlotEmptyCellsTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio con alcune celle vuote
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("B");
            // B3 è lasciato vuoto
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B4"].PutValue(30);

            // Aggiungi grafico
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Imposta l'intervallo dei dati
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Dimostra la proprietà PlotEmptyCellsType
            chart.PlotEmptyCellsType = Aspose.Cells.Charts.PlotEmptyCellsType.Zero;
            Console.WriteLine("PlotEmptyCellsType set to: " + chart.PlotEmptyCellsType);

            // Salva la cartella di lavoro
            workbook.Save("PlotEmptyCellsTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PlotEmptyCellsType](../../plotemptycellstype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


