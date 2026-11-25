---
title: "PageSetup.GetFirstPageHeader"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PageSetup. Ottiene uno script che formatta l'intestazione della prima pagina di un file Excel"
type: docs
url: /it/net/aspose.cells/pagesetup/getfirstpageheader/
---
## PageSetup.GetFirstPageHeader method

Ottiene uno script che formatta l'intestazione della prima pagina di un file Excel.

```csharp
public string GetFirstPageHeader(int section)
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
    public class PageSetupMethodGetFirstPageHeaderWithInt32Demo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi a PageSetup
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Abilita intestazione/piè di pagina diversi per la prima pagina
            pageSetup.IsHFDiffFirst = true;
            
            // Imposta le sezioni dell'intestazione della prima pagina
            pageSetup.SetFirstPageHeader(0, "&LFirst Page Left Header");
            pageSetup.SetFirstPageHeader(1, "&CFirst Page Center Header");
            pageSetup.SetFirstPageHeader(2, "&RFirst Page Right Header");
            
            // Ottieni e visualizza le sezioni dell'intestazione della prima pagina
            Console.WriteLine("First Page Header Sections:");
            Console.WriteLine("Left: " + pageSetup.GetFirstPageHeader(0));
            Console.WriteLine("Center: " + pageSetup.GetFirstPageHeader(1));
            Console.WriteLine("Right: " + pageSetup.GetFirstPageHeader(2));
            
            // Salva la cartella di lavoro
            workbook.Save("PageSetupFirstPageHeaderDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


