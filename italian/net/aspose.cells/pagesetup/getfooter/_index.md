---
title: "PageSetup.GetFooter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PageSetup. Ottiene uno script che formatta il piè di pagina di un file Excel"
type: docs
url: /it/net/aspose.cells/pagesetup/getfooter/
---
## PageSetup.GetFooter method

Ottiene uno script che formatta il piè di pagina di un file Excel.

```csharp
public string GetFooter(int section)
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
    public class PageSetupMethodGetFooterWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta diverse sezioni del piè di pagina
            worksheet.PageSetup.SetFooter(1, "odd");
            worksheet.PageSetup.SetFirstPageFooter(1, "first");
            worksheet.PageSetup.SetEvenFooter(1, "even");

            // Ottieni e visualizza le sezioni del piè di pagina
            Console.WriteLine("First Page Footer: " + worksheet.PageSetup.GetFirstPageFooter(1));
            Console.WriteLine("Even Page Footer: " + worksheet.PageSetup.GetEvenFooter(1));
            Console.WriteLine("Odd Page Footer: " + worksheet.PageSetup.GetFooter(1));
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


