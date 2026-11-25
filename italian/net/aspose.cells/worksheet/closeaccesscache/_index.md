---
title: "Worksheet.CloseAccessCache"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Worksheet. Chiude la sessione che utilizza le cache per accedere ai dati in questo foglio di lavoro"
type: docs
url: /it/net/aspose.cells/worksheet/closeaccesscache/
---
## Worksheet.CloseAccessCache method

Chiude la sessione che utilizza cache per accedere ai dati in questo foglio di lavoro.

```csharp
public void CloseAccessCache(AccessCacheOptions opts)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| opts | AccessCacheOptions | opzioni di accesso ai dati |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCloseAccessCacheWithAccessCacheOptionsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Popola le celle con dati di esempio
            for (int i = 0; i < 1000; i++)
            {
                cells[i, 0].PutValue(i % 10);
            }

            // Aggiungi formattazione condizionale
            FormatConditionCollection fcs = sheet.ConditionalFormattings[sheet.ConditionalFormattings.Add()];
            fcs.AddArea(CellArea.CreateCellArea(0, 0, 999, 0));
            fcs.AddCondition(FormatConditionType.ColorScale);

            // Abilita la cache di accesso per la formattazione condizionale
            sheet.StartAccessCache(AccessCacheOptions.ConditionalFormatting);

            // Esegui operazioni con accesso in cache
            Random random = new Random();
            for (int i = 0; i < 100; i++)
            {
                int r = random.Next(0, 1000);
                var style = cells[r, 0].GetDisplayStyle();
                Console.WriteLine($"Cell ({r},0) style: {style.ForegroundArgbColor:X}");
            }

            // Chiudi la cache di accesso
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


