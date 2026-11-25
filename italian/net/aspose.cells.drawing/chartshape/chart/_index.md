---
title: "ChartShape.Chart"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartShape. Restituisce un oggetto Chart che rappresenta il grafico contenuto nell'oggetto"
type: docs
url: /it/net/aspose.cells.drawing/chartshape/chart/
---
## ChartShape.Chart property

Restituisce un oggetto Chart che rappresenta il grafico contenuto nell'oggetto.

```csharp
public Chart Chart { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class ChartShapePropertyChartDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["A4"].PutValue("Grains");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ottieni l'istanza di ChartShape
            ChartShape chartShape = (ChartShape)chart.ChartObject;

            // Accedi alla proprietà Chart (sola lettura)
            Chart accessedChart = chartShape.Chart;

            // Visualizza le proprietà del grafico
            Console.WriteLine("Chart Name: " + accessedChart.Name);
            Console.WriteLine("Chart Type: " + accessedChart.Type);
            Console.WriteLine("Show Legend: " + accessedChart.ShowLegend);

            // Modifica le proprietà del grafico tramite l'oggetto Chart
            accessedChart.Name = "Sales Chart";
            accessedChart.ShowLegend = false;
            accessedChart.Title.Text = "Product Sales Distribution";

            // Cambia il tipo di grafico
            accessedChart.Type = ChartType.Pie;

            // Salva il risultato
            workbook.Save("ChartShapePropertyChartDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Chart](../../../aspose.cells.charts/chart/)
* class [ChartShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


