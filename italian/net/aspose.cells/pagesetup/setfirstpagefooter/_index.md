---
title: "PageSetup.SetFirstPageFooter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PageSetup. Imposta uno script che formatta il piè di pagina della prima pagina di un file Excel"
type: docs
url: /it/net/aspose.cells/pagesetup/setfirstpagefooter/
---
## PageSetup.SetFirstPageFooter method

Imposta uno script che formatta il piè di pagina della prima pagina di un file Excel.

```csharp
public void SetFirstPageFooter(int section, string footerScript)
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
    public class PageSetupMethodSetFirstPageFooterWithInt32StringDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ottieni l'oggetto PageSetup
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Imposta intestazioni/piè di pagina diversi per la prima pagina
            pageSetup.IsHFDiffFirst = true;
            
            // Imposta il piè di pagina della prima pagina con indice di sezione e testo
            pageSetup.SetFirstPageFooter(0, "First Page Footer Text");
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
            
            Console.WriteLine("First page footer set successfully.");
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


