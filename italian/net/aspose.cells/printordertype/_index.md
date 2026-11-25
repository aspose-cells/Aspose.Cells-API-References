---
title: "Enum PrintOrderType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.PrintOrderType enum. Rappresenta le costanti dell'ordine di stampa"
type: docs
url: /it/net/aspose.cells/printordertype/
---
## PrintOrderType enumeration

Rappresenta le costanti dell'ordine di stampa.

```csharp
public enum PrintOrderType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| DownThenOver | `0` | Giù, poi a destra |
| OverThenDown | `1` | A destra, poi giù |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PrintOrderTypeDemo
    {
        public static void PrintOrderTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi all'oggetto PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // Imposta l'ordine di stampa su DownThenOver
            pageSetup.Order = PrintOrderType.DownThenOver;

            // Imposta alcune altre proprietà di configurazione della pagina a scopo dimostrativo
            pageSetup.PrintArea = "A1:D10";
            pageSetup.PrintTitleRows = "$1:$1";
            pageSetup.PrintTitleColumns = "$A:$A";
            pageSetup.CenterHorizontally = true;
            pageSetup.CenterVertically = true;

            // Salva la cartella di lavoro
            workbook.Save("PrintOrderTypeExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


