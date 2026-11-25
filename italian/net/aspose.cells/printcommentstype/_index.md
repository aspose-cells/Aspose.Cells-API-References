---
title: "Enum PrintCommentsType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.PrintCommentsType enum. Rappresenta il modo in cui i commenti vengono stampati con il foglio"
type: docs
url: /it/net/aspose.cells/printcommentstype/
---
## PrintCommentsType enumeration

Rappresenta il modo in cui i commenti vengono stampati con il foglio.

```csharp
public enum PrintCommentsType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| PrintInPlace | `0` | Rappresenta la stampa dei commenti così come visualizzati sul foglio. |
| PrintNoComments | `1` | Rappresenta il non stampare i commenti. |
| PrintSheetEnd | `2` | Rappresenta la stampa dei commenti alla fine del foglio. |
| PrintWithThreadedComments | `3` | Rappresenta la stampa dei commenti così come visualizzati sul foglio includendo i commenti in thread. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PrintCommentsTypeDemo
    {
        public static void PrintCommentsTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni commenti al foglio di lavoro
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a comment.";

            commentIndex = worksheet.Comments.Add("B2");
            comment = worksheet.Comments[commentIndex];
            comment.Note = "This is another comment.";

            // Imposta il tipo di stampa dei commenti nella configurazione di pagina
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.PrintComments = PrintCommentsType.PrintSheetEnd;

            // Salva la cartella di lavoro in un file
            workbook.Save("PrintCommentsTypeExample.xlsx");

            Console.WriteLine("Workbook saved successfully with comments printed at the end of the sheet.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


