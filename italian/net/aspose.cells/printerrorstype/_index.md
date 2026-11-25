---
title: "Enum PrintErrorsType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.PrintErrorsType enum. Rappresenta le costanti di errore di stampa"
type: docs
url: /it/net/aspose.cells/printerrorstype/
---
## PrintErrorsType enumeration

Rappresenta le costanti di stampa degli errori.

```csharp
public enum PrintErrorsType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| PrintErrorsBlank | `0` | Indica di non stampare gli errori. |
| PrintErrorsDash | `1` | Indica di stampare gli errori come \"--\". |
| PrintErrorsDisplayed | `2` | Indica di stampare gli errori così come visualizzati. |
| PrintErrorsNA | `3` | Indica di stampare gli errori come \"#N/A\". |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PrintErrorsTypeDemo
    {
        public static void PrintErrorsTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi al PageSetup del foglio di lavoro
            PageSetup pageSetup = worksheet.PageSetup;

            // Imposta diversi tipi di errore di stampa
            pageSetup.PrintErrors = PrintErrorsType.PrintErrorsBlank;
            workbook.Save("PrintErrorsBlank.xlsx");

            pageSetup.PrintErrors = PrintErrorsType.PrintErrorsDash;
            workbook.Save("PrintErrorsDash.xlsx");

            pageSetup.PrintErrors = PrintErrorsType.PrintErrorsDisplayed;
            workbook.Save("PrintErrorsDisplayed.xlsx");

            pageSetup.PrintErrors = PrintErrorsType.PrintErrorsNA;
            workbook.Save("PrintErrorsNA.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


