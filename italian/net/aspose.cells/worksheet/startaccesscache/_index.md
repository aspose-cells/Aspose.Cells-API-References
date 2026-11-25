---
title: "Worksheet.StartAccessCache"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Worksheet. Avvia la sessione che utilizza le cache per accedere ai dati in questo foglio di lavoro"
type: docs
url: /it/net/aspose.cells/worksheet/startaccesscache/
---
## Worksheet.StartAccessCache method

Avvia la sessione che utilizza cache per accedere ai dati in questo worksheet.

```csharp
public void StartAccessCache(AccessCacheOptions opts)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| opts | AccessCacheOptions | opzioni di accesso ai dati |

### Osservazioni

Dopo aver terminato l'accesso ai dati, [`CloseAccessCache`](../closeaccesscache/) dovrebbe essere invocato con le stesse opzioni per cancellare tutte le cache e ripristinare la modalità di accesso normale.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodStartAccessCacheWithAccessCacheOptionsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Imposta lo stile predefinito
            Style style = wb.DefaultStyle;
            style.Font.Size = 10;
            wb.DefaultStyle = style;

            // Aggiungi formattazione condizionale
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            FormatConditionCollection fcc = cfc[cfc.Add()];
            fcc.AddArea(CellArea.CreateCellArea(0, 0, 10, 10));
            fcc.AddCondition(FormatConditionType.DuplicateValues);
            FormatCondition fc = fcc[0];
            fc.Style.Font.Size = 16;

            // Popola alcuni dati
            Cells cells = sheet.Cells;
            for (int i = 0; i < 10; i++)
            {
                cells[0, i].PutValue("A");
                cells[i, 0].PutValue(i);
            }

            // Avvia la cache di accesso per migliori prestazioni
            sheet.StartAccessCache(AccessCacheOptions.ConditionalFormatting);

            // Verifica gli stili
            for (int i = 0; i < 10; i++)
            {
                Console.WriteLine($"Cell[0,{i}] Font Size: {cells[0, i].GetDisplayStyle().Font.Size}");
                Console.WriteLine($"Cell[{i},0] Font Size: {cells[i, 0].GetDisplayStyle().Font.Size}");
            }

            // Chiudi la cache al termine
            sheet.CloseAccessCache(AccessCacheOptions.ConditionalFormatting);
        }
    }
}
```

### Vedi anche

* enum [AccessCacheOptions](../../accesscacheoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


