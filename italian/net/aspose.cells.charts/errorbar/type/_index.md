---
title: "ErrorBar.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ErrorBar. Rappresenta il tipo di quantità della barra di errore"
type: docs
url: /it/net/aspose.cells.charts/errorbar/type/
---
## ErrorBar.Type property

Rappresenta il tipo di quantità della barra di errore.

```csharp
public ErrorBarType Type { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ErrorBarPropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Aggiungi dati di esempio
            ws.Cells["A1"].PutValue(5);
            ws.Cells["A2"].PutValue(3);
            
            // Crea un grafico
            int chartIndex = ws.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = ws.Charts[chartIndex];
            
            // Aggiungi dati della serie
            chart.NSeries.Add("A3:A10", true);
            Series series = chart.NSeries[0];
            
            // Imposta il tipo e i valori della barra di errore personalizzata
            series.YErrorBar.Type = ErrorBarType.Custom;
            series.YErrorBar.PlusValue = "=Sheet1!A1";
            series.YErrorBar.MinusValue = "=Sheet1!A2";
            
            // Salva la cartella di lavoro
            wb.Save("ErrorBarDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ErrorBarType](../../errorbartype/)
* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


