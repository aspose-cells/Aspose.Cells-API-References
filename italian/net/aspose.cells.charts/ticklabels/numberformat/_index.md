---
title: "TickLabels.NumberFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TickLabels. Rappresenta la stringa di formato per l'oggetto TickLabels"
type: docs
url: /it/net/aspose.cells.charts/ticklabels/numberformat/
---
## TickLabels.NumberFormat property

Rappresenta la stringa di formato per l'oggetto TickLabels.

```csharp
public string NumberFormat { get; set; }
```

### Osservazioni

La stringa di formattazione è la stessa di una stringa di formato personalizzato impostata su una cella. Ad esempio, "$0".

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyNumberFormatDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(1.2345);
            worksheet.Cells["A3"].PutValue(2.3456);
            worksheet.Cells["A4"].PutValue(3.4567);

            // Crea un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("A2:A4", true);

            // Imposta il formato numerico per le etichette dei tick dell'asse dei valori
            chart.ValueAxis.TickLabels.NumberFormat = "0.00";

            // Salva la cartella di lavoro
            workbook.Save("TickLabelsNumberFormatDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


