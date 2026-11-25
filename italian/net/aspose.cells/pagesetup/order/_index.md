---
title: "PageSetup.Order"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PageSetup proprietà. Rappresenta l'ordine che Microsoft Excel utilizza per numerare le pagine durante la stampa di un foglio di lavoro di grandi dimensioni"
type: docs
url: /it/net/aspose.cells/pagesetup/order/
---
## PageSetup.Order property

Rappresenta l'ordine che Microsoft Excel utilizza per numerare le pagine durante la stampa di un foglio di lavoro di grandi dimensioni.

```csharp
public PrintOrderType Order { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyOrderDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Imposta l'ordine di stampa su DownThenOver
            sheet.PageSetup.Order = PrintOrderType.DownThenOver;
            Console.WriteLine("Print order set to: " + sheet.PageSetup.Order);

            // Salva la cartella di lavoro in diversi formati
            workbook.Save("output_DownThenOver.xlsx", SaveFormat.Xlsx);
            workbook.Save("output_DownThenOver.xls", SaveFormat.Excel97To2003);

            // Modifica l'ordine di stampa in OverThenDown
            sheet.PageSetup.Order = PrintOrderType.OverThenDown;
            Console.WriteLine("Print order changed to: " + sheet.PageSetup.Order);

            // Salva nuovamente con formati diversi
            workbook.Save("output_OverThenDown.xlsx", SaveFormat.Xlsx);
            workbook.Save("output_OverThenDown.xls", SaveFormat.Excel97To2003);
        }
    }
}
```

### Vedi anche

* enum [PrintOrderType](../../printordertype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


