---
title: "PageSetup.SetEvenHeader"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PageSetup metodo. Imposta uno script che formatta l'intestazione di pagina pari di un file Excel. Ha effetto solo in Excel 2007 quando IsHFDiffOddEven è true"
type: docs
url: /it/net/aspose.cells/pagesetup/setevenheader/
---
## PageSetup.SetEvenHeader method

Imposta uno script che formatta l'intestazione pari di un file Excel. Ha effetto solo in Excel 2007 quando IsHFDiffOddEven è true.

```csharp
public void SetEvenHeader(int section, string headerScript)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| section | Int32 | 0: Sezione sinistra, 1: Sezione centrale, 2: Sezione destra. |
| headerScript | String | Script di formattazione dell'intestazione. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetEvenHeaderWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Abilita intestazioni/piè di pagina diversi per le pagine dispari e pari
            pageSetup.IsHFDiffOddEven = true;

            // Imposta l'intestazione di pagina pari con indice di sezione e testo
            pageSetup.SetEvenHeader(1, "Even Page Header - Center Section");
            pageSetup.SetEvenHeader(0, "Even Page Header - Left Section");
            pageSetup.SetEvenHeader(2, "Even Page Header - Right Section");

            // Salva la cartella di lavoro
            workbook.Save("PageSetup_SetEvenHeaderExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


