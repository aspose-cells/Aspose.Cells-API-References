---
title: "Chart.PrintSize"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Chart. Ottiene e imposta la dimensione stampata del grafico"
type: docs
url: /it/net/aspose.cells.charts/chart/printsize/
---
## Chart.PrintSize property

Ottiene e imposta la dimensione stampata del grafico.

```csharp
public PrintSizeType PrintSize { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPrintSizeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Configura le impostazioni di stampa
            chart.PrintSize = PrintSizeType.Full;
            chart.SizeWithWindow = false;
            chart.AutoScaling = false;

            // Salva la cartella di lavoro
            workbook.Save("ChartPrintSizeDemo.pdf", SaveFormat.Pdf);
        }
    }
}
```

### Vedi anche

* enum [PrintSizeType](../../../aspose.cells/printsizetype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


