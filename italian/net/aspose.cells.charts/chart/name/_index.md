---
title: "Chart.Name"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Chart. Ottiene e imposta il nome del grafico"
type: docs
url: /it/net/aspose.cells.charts/chart/name/
---
## Chart.Name property

Ottiene e imposta il nome del grafico.

```csharp
public string Name { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Visualizza il nome del grafico
            Console.WriteLine("Chart Name: " + chart.Name);

            // Aggiungi un altro grafico e visualizza il suo nome
            int chartIndex2 = worksheet.Charts.Add(ChartType.Pie, 20, 0, 30, 5);
            Aspose.Cells.Charts.Chart chart2 = worksheet.Charts[chartIndex2];
            chart2.NSeries.Add("B2:B4", true);
            chart2.NSeries.CategoryData = "A2:A4";
            Console.WriteLine("Second Chart Name: " + chart2.Name);
        }
    }
}
```

### Vedi anche

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


