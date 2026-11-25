---
title: "PageSetup.GetEvenHeader"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PageSetup. Ottiene uno script che formatta l'intestazione pari di un file Excel"
type: docs
url: /it/net/aspose.cells/pagesetup/getevenheader/
---
## PageSetup.GetEvenHeader method

Ottiene uno script che formatta l'intestazione pari di un file Excel.

```csharp
public string GetEvenHeader(int section)
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
    public class PageSetupMethodGetEvenHeaderWithInt32Demo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Abilita intestazioni/piedini di pagina diversi per pari e dispari
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.IsHFDiffOddEven = true;
            
            // Imposta l'intestazione pari della pagina
            pageSetup.SetEvenHeader(0, "&CEven Page Header Center");
            pageSetup.SetEvenHeader(1, "&LEven Page Header Left");
            pageSetup.SetEvenHeader(2, "&REven Page Header Right");
            
            // Ottieni e stampa le intestazioni pari della pagina
            Console.WriteLine("Even Header Center: " + pageSetup.GetEvenHeader(0));
            Console.WriteLine("Even Header Left: " + pageSetup.GetEvenHeader(1));
            Console.WriteLine("Even Header Right: " + pageSetup.GetEvenHeader(2));
            
            // Salva la cartella di lavoro
            workbook.Save("PageSetup_GetEvenHeaderDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


