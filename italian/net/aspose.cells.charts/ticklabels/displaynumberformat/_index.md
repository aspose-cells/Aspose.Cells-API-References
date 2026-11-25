---
title: "TickLabels.DisplayNumberFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TickLabels. Ottiene e imposta il formato numerico di visualizzazione delle etichette dei tick"
type: docs
url: /it/net/aspose.cells.charts/ticklabels/displaynumberformat/
---
## TickLabels.DisplayNumberFormat property

Ottiene e imposta il formato numerico di visualizzazione delle etichette dei segni.

```csharp
public string DisplayNumberFormat { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyDisplayNumberFormatDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(DateTime.Now);
            worksheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            
            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("A2:A3", true);
            chart.NSeries.CategoryData = "B2:B3";
            
            // Imposta il formato numerico tramite la proprietà NumberFormat invece
            chart.CategoryAxis.TickLabels.NumberFormat = "m/d/yyyy";
            chart.ValueAxis.TickLabels.NumberFormat = "#,##0";
            
            // Salva la cartella di lavoro
            workbook.Save("TickLabelsDisplayNumberFormatDemo.xlsx");
            
            Console.WriteLine("DisplayNumberFormat for CategoryAxis: " + 
                chart.CategoryAxis.TickLabels.DisplayNumberFormat);
            Console.WriteLine("DisplayNumberFormat for ValueAxis: " + 
                chart.ValueAxis.TickLabels.DisplayNumberFormat);
        }
    }
}
```

### Vedi anche

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


