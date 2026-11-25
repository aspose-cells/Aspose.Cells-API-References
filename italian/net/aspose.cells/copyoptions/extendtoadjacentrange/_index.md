---
title: "CopyOptions.ExtendToAdjacentRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CopyOptions. Indica se estendere gli intervalli quando si copia l'intervallo in un intervallo adiacente"
type: docs
url: /it/net/aspose.cells/copyoptions/extendtoadjacentrange/
---
## CopyOptions.ExtendToAdjacentRange property

Indica se estendere gli intervalli quando si copia l'intervallo a quello adiacente.

```csharp
public bool ExtendToAdjacentRange { get; set; }
```

### Osservazioni

Se è true, estende solo l'intervallo del collegamento ipertestuale, senza aggiungere un nuovo collegamento ipertestuale quando si copiano i collegamenti ipertestuali in righe adiacenti.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyExtendToAdjacentRangeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // Aggiungi un collegamento ipertestuale alla cella A1
            ws.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // Crea le opzioni di copia e imposta ExtendToAdjacentRange su true
            CopyOptions copyOptions = new CopyOptions();
            copyOptions.ExtendToAdjacentRange = true;

            // Copia la riga 0 nella riga 1 con le opzioni di copia
            ws.Cells.CopyRows(ws.Cells, 0, 1, 1, copyOptions);

            // Verifica che il collegamento ipertestuale sia stato esteso all'intervallo adiacente
            Console.WriteLine("Hyperlink count after copy: " + ws.Hyperlinks.Count);
        }
    }
}
```

### Vedi anche

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


