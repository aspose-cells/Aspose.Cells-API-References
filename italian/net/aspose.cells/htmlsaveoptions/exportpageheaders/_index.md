---
title: "HtmlSaveOptions.ExportPageHeaders"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se esportare le intestazioni di pagina"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/exportpageheaders/
---
## HtmlSaveOptions.ExportPageHeaders property

Indica se esportare le intestazioni di pagina.

```csharp
public bool ExportPageHeaders { get; set; }
```

### Osservazioni

Funziona solo quando [`SaveAsSingleFile`](../saveassinglefile/) è True.

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportPageHeadersDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta l'intestazione della pagina
            worksheet.PageSetup.SetHeader(0, "Sample Header Text");
            
            // Aggiungi alcuni dati al worksheet
            worksheet.Cells["A1"].PutValue("This is a test");
            
            // Configura le opzioni di salvataggio HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                SaveAsSingleFile = true,
                ShowAllSheets = true,
                ExportPageHeaders = true  // This is the key property being demonstrated
            };
            
            // Salva la cartella di lavoro come HTML
            string outputPath = "output_with_headers.html";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("HTML file with page headers exported successfully.");
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


