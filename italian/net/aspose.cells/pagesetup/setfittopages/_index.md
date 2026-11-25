---
title: "PageSetup.SetFitToPages"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PageSetup metodo. Imposta il numero di pagine a cui il foglio di lavoro sarà ridimensionato quando stampato"
type: docs
url: /it/net/aspose.cells/pagesetup/setfittopages/
---
## PageSetup.SetFitToPages method

Imposta il numero di pagine a cui il foglio di lavoro verrà ridimensionato quando viene stampato.

```csharp
public void SetFitToPages(int wide, int tall)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| largo | Int32 | Pagine larghe. |
| alto | Int32 | Altezza in pagine. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetFitToPagesWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Accedi al PageSetup del primo foglio di lavoro
            PageSetup setup = workbook.Worksheets[0].PageSetup;
            
            // Imposta le impostazioni di adattamento alle pagine
            setup.SetFitToPages(2, 3);
            
            // Verifica e visualizza le impostazioni
            Console.WriteLine("IsPercentScale: " + setup.IsPercentScale);
            Console.WriteLine("FitToPagesWide: " + setup.FitToPagesWide);
            Console.WriteLine("FitToPagesTall: " + setup.FitToPagesTall);
            
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


