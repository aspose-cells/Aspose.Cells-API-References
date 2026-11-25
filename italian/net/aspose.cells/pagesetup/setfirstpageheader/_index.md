---
title: "PageSetup.SetFirstPageHeader"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PageSetup metodo. Imposta uno script che formatta l'intestazione di prima pagina di un file Excel. Ha effetto solo in Excel 2007 quando IsHFDiffFirst è true"
type: docs
url: /it/net/aspose.cells/pagesetup/setfirstpageheader/
---
## PageSetup.SetFirstPageHeader method

Imposta uno script per formattare l'intestazione della prima pagina di un file Excel. Ha effetto solo in Excel 2007 quando IsHFDiffFirst è true.

```csharp
public void SetFirstPageHeader(int section, string headerScript)
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
    public class PageSetupMethodSetFirstPageHeaderWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Imposta l'intestazione di prima pagina con numero di sezione e testo dell'intestazione
            pageSetup.SetFirstPageHeader(2, "&CHeader Text");

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


