---
title: "DataLabels.Number"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataLabels. Ottiene e imposta il formato numerico incorporato"
type: docs
url: /it/net/aspose.cells.charts/datalabels/number/
---
## DataLabels.Number property

Ottiene e imposta il formato numerico incorporato.

```csharp
public int Number { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyNumberDemo
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
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Bar, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ottieni la prima serie e abilita le etichette dati
            Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            
            // Accedi alle proprietà delle etichette dati
            DataLabels dataLabels = series.DataLabels;
            
            // Dimostra l'uso della proprietà Number
            Console.WriteLine("Original Number format: " + dataLabels.NumberFormat);
            Console.WriteLine("Original Number property value: " + dataLabels.Number);
            
            // Modifica il formato numerico
            dataLabels.Number = 2; // Currency format
            dataLabels.NumberFormat = "$#,##0.00";
            
            Console.WriteLine("Modified Number format: " + dataLabels.NumberFormat);
            Console.WriteLine("Modified Number property value: " + dataLabels.Number);

            // Salva la cartella di lavoro
            workbook.Save("DataLabelsNumberDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


