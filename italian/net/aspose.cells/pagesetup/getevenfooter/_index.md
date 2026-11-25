---
title: "PageSetup.GetEvenFooter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PageSetup. Ottiene uno script che formatta il piè di pagina pari di un file Excel"
type: docs
url: /it/net/aspose.cells/pagesetup/getevenfooter/
---
## PageSetup.GetEvenFooter method

Ottiene uno script che formatta il piè di pagina pari di un file Excel.

```csharp
public string GetEvenFooter(int section)
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
    public class PageSetupMethodGetEvenFooterWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Abilita intestazioni/piè di pagina diversi per le pagine dispari e pari
            pageSetup.IsHFDiffOddEven = true;
            
            // Imposta il piè di pagina pari
            pageSetup.SetEvenFooter(0, "Even Page Footer");
            
            // Ottieni e visualizza il piè di pagina pari
            string evenFooter = pageSetup.GetEvenFooter(0);
            Console.WriteLine("Even Footer: " + evenFooter);
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


