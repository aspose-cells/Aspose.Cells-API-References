---
title: "ErrorBar.DisplayType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ErrorBar. Rappresenta il tipo di visualizzazione della barra di errore"
type: docs
url: /it/net/aspose.cells.charts/errorbar/displaytype/
---
## ErrorBar.DisplayType property

Rappresenta il tipo di visualizzazione della barra di errore.

```csharp
public ErrorBarDisplayType DisplayType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ErrorBarPropertyDisplayTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Aggiungi serie
            chart.NSeries.Add("A2:A4", true);
            chart.NSeries.CategoryData = "B2:B4";

            // Imposta il tipo di visualizzazione della barra di errore
            chart.NSeries[0].YErrorBar.DisplayType = ErrorBarDisplayType.Plus;

            // Salva la cartella di lavoro
            workbook.Save("ErrorBarDisplayTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* enum [ErrorBarDisplayType](../../errorbardisplaytype/)
* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


