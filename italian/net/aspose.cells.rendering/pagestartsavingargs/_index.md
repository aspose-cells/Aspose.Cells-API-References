---
title: "Classe PageStartSavingArgs"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Rendering.PageStartSavingArgs. Informazioni per l'inizio del processo di salvataggio di una pagina"
type: docs
url: /it/net/aspose.cells.rendering/pagestartsavingargs/
---
## PageStartSavingArgs class

Informazioni per l'avvio del processo di salvataggio di una pagina.

```csharp
public class PageStartSavingArgs : PageSavingArgs
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [IsToOutput](../../aspose.cells.rendering/pagestartsavingargs/istooutput/) { get; set; } | Ottiene o imposta un valore che indica se la pagina deve essere esportata. Il valore predefinito è true. |
| [PageCount](../../aspose.cells.rendering/pagesavingargs/pagecount/) { get; } | Conteggio totale delle pagine.(Ereditato da [`PageSavingArgs`](../pagesavingargs/).) |
| [PageIndex](../../aspose.cells.rendering/pagesavingargs/pageindex/) { get; } | Indice della pagina corrente, basato su zero.(Ereditato da [`PageSavingArgs`](../pagesavingargs/).) |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingClassPageStartSavingArgsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].PutValue("Hello World");
            
            PdfSaveOptions options = new PdfSaveOptions();
            options.PageSavingCallback = new CustomPageSavingCallback();
            
            workbook.Save("output.pdf", options);
        }
    }
    
    public class CustomPageSavingCallback : IPageSavingCallback
    {
        public void PageStartSaving(PageStartSavingArgs args)
        {
            Console.WriteLine($"Starting to save page {args.PageIndex}");
        }
        
        public void PageEndSaving(PageEndSavingArgs args)
        {
            // Implementazione opzionale
        }
    }
}
```

### Vedi anche

* class [PageSavingArgs](../pagesavingargs/)
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


