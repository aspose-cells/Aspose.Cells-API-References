---
title: "Enum TxtValueQuoteType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.TxtValueQuoteType enum. Specifica il tipo di utilizzo delle virgolette per i valori nei file di formato testo"
type: docs
url: /it/net/aspose.cells/txtvaluequotetype/
---
## TxtValueQuoteType enumeration

Specifica il tipo di utilizzo delle virgolette per i valori nei file di formato testo.

```csharp
public enum TxtValueQuoteType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Normal | `0` | Tutti i valori che contengono caratteri speciali come virgolette, carattere separatore saranno racchiusi tra virgolette. Stesso comportamento di MS Excel per l'esportazione di file di testo. |
| Always | `1` | Tutti i valori saranno sempre racchiusi tra virgolette. |
| Minimum | `2` | Racchiudi tra virgolette i valori solo quando necessario. Ad esempio, se un valore contiene una virgoletta ma la virgoletta non è all'inizio di questo valore, il valore non sarà racchiuso tra virgolette. |
| Never | `3` | Nessun valore sarà racchiuso tra virgolette. Il file di testo esportato con questo tipo potrebbe non essere letto correttamente perché le virgolette necessarie sono assenti. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TxtValueQuoteTypeDemo
    {
        public static void TxtValueQuoteTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati al worksheet
            worksheet.Cells[0, 0].Value = "Name";
            worksheet.Cells[0, 1].Value = "Age";
            worksheet.Cells[1, 0].Value = "John Doe";
            worksheet.Cells[1, 1].Value = 30;
            worksheet.Cells[2, 0].Value = "Jane Smith";
            worksheet.Cells[2, 1].Value = 25;

            // Crea TxtSaveOptions e imposta il QuoteType
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.QuoteType = TxtValueQuoteType.Always;

            // Salva la cartella di lavoro come file di testo con il tipo di virgolette specificato
            workbook.Save("TxtValueQuoteTypeExample.txt", saveOptions);

            Console.WriteLine("Workbook saved with TxtValueQuoteType.Always");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


