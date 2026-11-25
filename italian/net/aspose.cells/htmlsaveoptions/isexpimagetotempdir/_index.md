---
title: "HtmlSaveOptions.IsExpImageToTempDir"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se esportare i file immagine nella directory temporanea. Solo per il salvataggio in un flusso html"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/isexpimagetotempdir/
---
## HtmlSaveOptions.IsExpImageToTempDir property

Indica se esportare i file immagine in una directory temporanea. Solo per il salvataggio in stream HTML.

```csharp
public bool IsExpImageToTempDir { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsExpImageToTempDirDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di esempio con un'immagine
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un'immagine di esempio al foglio di lavoro
            worksheet.Pictures.Add(0, 0, "https://www.aspose.com/templates/aspose/App_Themes/V3/images/cells/header/aspose_cells-for-net.png");

            // Imposta le opzioni di salvataggio HTML con IsExpImageToTempDir abilitato
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.IsExpImageToTempDir = true;
            options.ExportImagesAsBase64 = false; // Ensure images are exported as separate files

            // Salva la cartella di lavoro come HTML
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML saved with images exported to temp directory.");
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


