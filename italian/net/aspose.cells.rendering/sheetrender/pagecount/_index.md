---
title: "SheetRender.PageCount"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SheetRender. Ottiene il conteggio totale delle pagine del foglio di lavoro corrente"
type: docs
url: /it/net/aspose.cells.rendering/sheetrender/pagecount/
---
## SheetRender.PageCount property

Restituisce il conteggio totale delle pagine del foglio di lavoro corrente.

```csharp
public int PageCount { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderPropertyPageCountDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(30);
            cells["A3"].PutValue("Mary");
            cells["B3"].PutValue(25);
            cells["A4"].PutValue("Peter");
            cells["B4"].PutValue(35);

            // Imposta la configurazione della pagina per la stampa
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.PrintArea = "A1:B4";
            pageSetup.FitToPagesTall = 1;
            pageSetup.FitToPagesWide = 1;

            // Crea SheetRender con le opzioni predefinite
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            SheetRender render = new SheetRender(worksheet, options);

            // Visualizza il conteggio delle pagine
            Console.WriteLine("Page Count: " + render.PageCount);

            // Modifica la configurazione della pagina per forzare più pagine
            pageSetup.FitToPagesTall = 0;
            pageSetup.FitToPagesWide = 1;
            pageSetup.PrintArea = "A1:B100"; // Larger area than can fit on one page

            // Crea un nuovo SheetRender per ottenere il conteggio delle pagine aggiornato
            SheetRender newRender = new SheetRender(worksheet, options);
            Console.WriteLine("Updated Page Count: " + newRender.PageCount);
        }
    }
}
```

### Vedi anche

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


