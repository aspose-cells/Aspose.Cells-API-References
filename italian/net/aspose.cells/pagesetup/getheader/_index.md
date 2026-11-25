---
title: "PageSetup.GetHeader"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PageSetup. Ottiene uno script che formatta l'intestazione di un file Excel"
type: docs
url: /it/net/aspose.cells/pagesetup/getheader/
---
## PageSetup.GetHeader method

Ottiene uno script che formatta l'intestazione di un file Excel.

```csharp
public string GetHeader(int section)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| section | Int32 | 0: Sezione sinistra, 1: Sezione centrale, 2: Sezione destra. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodGetHeaderWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta l'intestazione per la sezione 2
            worksheet.PageSetup.SetHeader(2, "&8Report ID: TEST01\n你好Public");
            
            // Ottieni e stampa l'intestazione per la sezione 2
            string header = worksheet.PageSetup.GetHeader(2);
            Console.WriteLine("Header for section 2: " + header);
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


