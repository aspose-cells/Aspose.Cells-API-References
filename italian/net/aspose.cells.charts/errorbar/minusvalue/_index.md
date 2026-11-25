---
title: "ErrorBar.MinusValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ErrorBar. Rappresenta la quantità di errore negativa quando il tipo di barra di errore è Personalizzato"
type: docs
url: /it/net/aspose.cells.charts/errorbar/minusvalue/
---
## ErrorBar.MinusValue property

Rappresenta la quantità di errore negativa quando il tipo di barra di errore è Personalizzato.

```csharp
public string MinusValue { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ErrorBarPropertyMinusValueDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Values");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(5);
            worksheet.Cells["B1"].PutValue("Data");
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(15);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Aggiungi serie
            chart.NSeries.Add("B2:B3", true);

            // Configura le barre di errore
            ErrorBar errorBar = chart.NSeries[0].YErrorBar;
            errorBar.DisplayType = ErrorBarDisplayType.Both;
            errorBar.Type = ErrorBarType.Custom;
            errorBar.PlusValue = "=A2";
            errorBar.MinusValue = "=A3";

            // Salva la cartella di lavoro
            workbook.Save("ErrorBarMinusValueDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


