---
title: "HtmlSaveOptions.ExportImagesAsBase64"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Specifica se le immagini vengono salvate in formato Base64 in HTML, MHTML o EPUB."
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/exportimagesasbase64/
---
## HtmlSaveOptions.ExportImagesAsBase64 property

Specifica se le immagini vengono salvate in formato Base64 in HTML, MHTML o EPUB.

```csharp
public bool ExportImagesAsBase64 { get; set; }
```

### Osservazioni

Quando questa proprietà è impostata su true, i dati dell'immagine vengono esportati direttamente negli elementi img e non vengono creati file separati.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportImagesAsBase64Demo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un'immagine al foglio di lavoro
            worksheet.Pictures.Add(0, 0, "example.jpg");
            
            // Crea opzioni di salvataggio HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Imposta ExportImagesAsBase64 su true per incorporare le immagini come stringhe Base64.
            saveOptions.ExportImagesAsBase64 = true;
            
            // Salva la cartella di lavoro come HTML con immagini incorporate.
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML with embedded images saved successfully.");
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


