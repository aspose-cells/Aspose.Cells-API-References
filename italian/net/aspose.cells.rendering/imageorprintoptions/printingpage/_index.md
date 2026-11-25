---
title: "ImageOrPrintOptions.PrintingPage"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageOrPrintOptions. Indica quali pagine non saranno stampate"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/printingpage/
---
## ImageOrPrintOptions.PrintingPage property

Indica quali pagine non saranno stampate.

```csharp
public PrintingPageType PrintingPage { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyPrintingPageDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni dati al worksheet
            worksheet.Cells["A1"].PutValue("Test Data");
            worksheet.Cells["A2"].PutValue("Non-Blank Cell");
            worksheet.Cells["A5"].PutValue("Another Non-Blank Cell");
            
            // Crea opzioni di immagine/stampa
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PrintingPage = PrintingPageType.IgnoreBlank;
            
            // Esegui il rendering della cartella di lavoro con le opzioni
            WorkbookRender render = new WorkbookRender(workbook, options);
            
            // Restituisci il conteggio delle pagine (ignorerà le pagine vuote)
            Console.WriteLine("Page count with IgnoreBlank: " + render.PageCount);
            
            // Cambia al comportamento predefinito (includi tutte le pagine)
            options.PrintingPage = PrintingPageType.Default;
            render = new WorkbookRender(workbook, options);
            Console.WriteLine("Page count with Default: " + render.PageCount);
        }
    }
}
```

### Vedi anche

* enum [PrintingPageType](../../../aspose.cells/printingpagetype/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


