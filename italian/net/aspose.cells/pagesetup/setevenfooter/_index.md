---
title: "PageSetup.SetEvenFooter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PageSetup. Imposta uno script che formatta il piè di pagina delle pagine pari di un file Excel. Ha effetto solo in Excel 2007 quando IsHFDiffOddEven è true"
type: docs
url: /it/net/aspose.cells/pagesetup/setevenfooter/
---
## PageSetup.SetEvenFooter method

Imposta uno script che formatta il piè di pagina pari di un file Excel. Ha effetto solo in Excel 2007 quando IsHFDiffOddEven è true.

```csharp
public void SetEvenFooter(int section, string footerScript)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| section | Int32 | 0: Sezione sinistra, 1: Sezione centrale, 2: Sezione destra. |
| footerScript | String | Script di formattazione del piè di pagina. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetEvenFooterWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Abilita intestazioni/piè di pagina diversi per la prima e le pagine pari
            pageSetup.IsHFDiffFirst = true;
            pageSetup.IsHFDiffOddEven = true;

            // Imposta tipi di piè di pagina diversi
            pageSetup.SetEvenFooter(0, "Even Page Footer");
            pageSetup.SetFooter(0, "Odd Page Footer");
            pageSetup.SetFirstPageFooter(0, "First Page Footer");

            // Salva la cartella di lavoro
            workbook.Save("PageSetup_SetEvenFooter_Example.xlsx");

            Console.WriteLine("Workbook saved with even page footer set successfully.");
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


