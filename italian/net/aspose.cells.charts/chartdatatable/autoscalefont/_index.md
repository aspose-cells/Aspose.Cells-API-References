---
title: "ChartDataTable.AutoScaleFont"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartDataTable. True se il testo nell'oggetto cambia la dimensione del carattere quando la dimensione dell'oggetto cambia. Il valore predefinito è True"
type: docs
url: /it/net/aspose.cells.charts/chartdatatable/autoscalefont/
---
## ChartDataTable.AutoScaleFont property

True se il testo nell'oggetto cambia dimensione del carattere quando le dimensioni dell'oggetto cambiano. Il valore predefinito è True.

```csharp
public bool AutoScaleFont { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyAutoScaleFontDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Abilita tabella dati
            chart.ShowDataTable = true;
            
            // Accedi alle proprietà della tabella dati del grafico
            // Modo corretto per ottenere ChartDataTable quando ShowDataTable è true
            ChartDataTable dataTable = chart.ChartDataTable;
            
            // Dimostra la proprietà AutoScaleFont
            dataTable.AutoScaleFont = false; // Disable auto-scaling
            Console.WriteLine("AutoScaleFont (false): " + dataTable.AutoScaleFont);
            
            dataTable.AutoScaleFont = true; // Enable auto-scaling
            Console.WriteLine("AutoScaleFont (true): " + dataTable.AutoScaleFont);

            // Salva la cartella di lavoro
            workbook.Save("ChartDataTableAutoScaleFontDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


