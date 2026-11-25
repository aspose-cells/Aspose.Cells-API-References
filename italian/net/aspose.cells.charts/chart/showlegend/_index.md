---
title: "Chart.ShowLegend"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Chart. Ottiene o imposta un valore che indica se la legenda del grafico verrà visualizzata. Il valore predefinito è true"
type: docs
url: /it/net/aspose.cells.charts/chart/showlegend/
---
## Chart.ShowLegend property

Ottiene o imposta un valore che indica se la legenda del grafico verrà visualizzata. Il valore predefinito è vero.

```csharp
public bool ShowLegend { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyShowLegendDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue("Item");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Orange");
            sheet.Cells["A4"].PutValue("Banana");
            sheet.Cells["B1"].PutValue("Quantity");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Mostra la legenda per impostazione predefinita (true)
            Console.WriteLine("Legend initially visible: " + chart.ShowLegend);
            
            // Nascondi la legenda
            chart.ShowLegend = false;
            Console.WriteLine("Legend after setting to false: " + chart.ShowLegend);
            
            // Salva la cartella di lavoro
            workbook.Save("ChartLegendExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


