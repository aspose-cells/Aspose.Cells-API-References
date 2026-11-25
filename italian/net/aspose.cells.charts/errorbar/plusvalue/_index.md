---
title: "ErrorBar.PlusValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ErrorBar. Rappresenta la quantità di errore positiva quando il tipo di barra di errore è Personalizzato"
type: docs
url: /it/net/aspose.cells.charts/errorbar/plusvalue/
---
## ErrorBar.PlusValue property

Rappresenta la quantità di errore positiva quando il tipo di barra di errore è Personalizzato.

```csharp
public string PlusValue { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ErrorBarPropertyPlusValueDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(5);
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(40);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);

            // Configura le barre di errore
            ErrorBar errorBar = chart.NSeries[0].YErrorBar;
            errorBar.DisplayType = ErrorBarDisplayType.Both;
            errorBar.Type = ErrorBarType.Custom;
            errorBar.PlusValue = "=A2";  // Using PlusValue property
            errorBar.MinusValue = "=A3";

            // Salva la cartella di lavoro
            workbook.Save("ErrorBarPlusValueDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


