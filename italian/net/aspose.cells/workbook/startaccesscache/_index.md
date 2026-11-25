---
title: "Workbook.StartAccessCache"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Avvia la sessione che utilizza le cache per accedere ai dati"
type: docs
url: /it/net/aspose.cells/workbook/startaccesscache/
---
## Workbook.StartAccessCache method

Avvia la sessione che utilizza cache per accedere ai dati.

```csharp
public void StartAccessCache(AccessCacheOptions opts)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| opts | AccessCacheOptions | opzioni di accesso ai dati |

### Osservazioni

Se la cache dell'accesso ai dati specificati richiede che alcuni modelli di dati nel foglio di lavoro siano "read-only", allora i modelli di dati corrispondenti in ogni foglio di lavoro di questa cartella saranno considerati "read-only" e l'utente non dovrebbe modificarne alcuno. Dopo aver terminato l'accesso ai dati, [`CloseAccessCache`](../closeaccesscache/) dovrebbe essere invocato con le stesse opzioni per cancellare tutte le cache e ripristinare la modalità di accesso normale.

### Esempi

```csharp
using System;
using System.Drawing;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodStartAccessCacheWithAccessCacheOptionsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Aggiungi formattazione condizionale
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            int index = cfc.Add();
            cfc[index].Add(CellArea.CreateCellArea(0, 0, 5, 0),
                FormatConditionType.DuplicateValues, OperatorType.None, null, null);
            
            // Imposta lo stile per la formattazione condizionale
            Style style = cfc[0][0].Style;
            style.ForegroundColor = Color.Red;
            style.Pattern = BackgroundType.Solid;
            
            // Aggiungi alcune immagini incorporate
            Cells cells = sheet.Cells;
            byte[] img1 = File.ReadAllBytes("1.png");
            byte[] img2 = File.ReadAllBytes("2.png");
            cells[0, 0].EmbeddedImage = img1;
            cells[2, 0].EmbeddedImage = img2;
            cells[4, 0].EmbeddedImage = img1;

            // Avvia la cache di accesso per migliori prestazioni
            wb.StartAccessCache(AccessCacheOptions.All);
            
            // Accedi agli stili delle celle (sarà più veloce grazie alla cache)
            Console.WriteLine("A1 Pattern: " + cells[0, 0].GetDisplayStyle().Pattern);
            Console.WriteLine("A3 Pattern: " + cells[2, 0].GetDisplayStyle().Pattern);
            Console.WriteLine("A5 Pattern: " + cells[4, 0].GetDisplayStyle().Pattern);
            
            // Chiudi la cache al termine
            wb.CloseAccessCache(AccessCacheOptions.All);
        }
    }
}
```

### Vedi anche

* enum [AccessCacheOptions](../../accesscacheoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


