---
title: "ImageOrPrintOptions.PageIndex"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageOrPrintOptions. Ottiene o imposta l'indice basato su 0 della prima pagina da salvare"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/pageindex/
---
## ImageOrPrintOptions.PageIndex property

Ottiene o imposta l'indice basato su 0 della prima pagina da salvare.

```csharp
public int PageIndex { get; set; }
```

### Osservazioni

Il valore predefinito è 0.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyPageIndexDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungere dati di esempio a più pagine
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Data Row " + (i + 1);
            }

            // Configurare le opzioni immagine/stampa
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PageIndex = 1; // Start from second page (0-based index would be 1)
            options.PageCount = 1; // Only process one page

            // Crea il rendering del foglio per il primo foglio di lavoro
            SheetRender render = new SheetRender(worksheet, options);

            // Salvare in PDF utilizzando il metodo API corretto
            render.ToImage(0, "output.pdf");
            Console.WriteLine("Saved page 2 to PDF successfully.");
        }
    }
}
```

### Vedi anche

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


