---
title: "Series.IsFiltered"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. Indica se la serie è selezionata o filtrata. True indica che questa serie è filtrata e non verrà visualizzata nel grafico"
type: docs
url: /it/net/aspose.cells.charts/series/isfiltered/
---
## Series.IsFiltered property

Indica se la serie è selezionata o filtrata. Vero indica che questa serie è filtrata e non verrà visualizzata nel grafico.

```csharp
public bool IsFiltered { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyIsFilteredDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["A5"].PutValue("D");
            
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);
            
            worksheet.Cells["C1"].PutValue("Series2");
            worksheet.Cells["C2"].PutValue(15);
            worksheet.Cells["C3"].PutValue(25);
            worksheet.Cells["C4"].PutValue(35);
            worksheet.Cells["C5"].PutValue(45);
            
            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.Add("C2:C5", true);
            chart.NSeries.CategoryData = "A2:A5";
            
            // Dimostrare la proprietà IsFiltered
            Console.WriteLine("Initial Series Count: " + chart.NSeries.Count);
            
            // Filtrare la prima serie
            chart.NSeries[0].IsFiltered = true;
            Console.WriteLine("After filtering first series: " + chart.NSeries.Count);
            
            // Filtrare la seconda serie
            chart.NSeries[0].IsFiltered = true;
            Console.WriteLine("After filtering second series: " + chart.NSeries.Count);
            
            // Salva la cartella di lavoro
            workbook.Save("SeriesFilteredDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


