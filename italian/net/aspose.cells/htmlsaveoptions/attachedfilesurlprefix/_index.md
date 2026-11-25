---
title: "HtmlSaveOptions.AttachedFilesUrlPrefix"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Specifica il prefisso URL dei file allegati, come le immagini, nel file HTML. Solo per il salvataggio su stream HTML"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/attachedfilesurlprefix/
---
## HtmlSaveOptions.AttachedFilesUrlPrefix property

Specifica il prefisso Url dei file allegati, come le immagini, nel file html. Solo per il salvataggio in stream html.

```csharp
public string AttachedFilesUrlPrefix { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyAttachedFilesUrlPrefixDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test HTML Export");

            // Imposta le opzioni di salvataggio HTML con AttachedFilesUrlPrefix
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            saveOptions.AttachedFilesUrlPrefix = "www.aspose.com";

            // Salva la cartella di lavoro con le opzioni HTML
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);

            Console.WriteLine("HTML file saved with AttachedFilesUrlPrefix: " + saveOptions.AttachedFilesUrlPrefix);
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


