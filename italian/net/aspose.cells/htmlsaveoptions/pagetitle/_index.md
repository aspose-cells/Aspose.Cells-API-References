---
title: "HtmlSaveOptions.PageTitle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Il titolo della pagina html. Solo per il salvataggio in uno stream html"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/pagetitle/
---
## HtmlSaveOptions.PageTitle property

Il titolo della pagina HTML. Solo per il salvataggio in stream HTML.

```csharp
public string PageTitle { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyPageTitleDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample HTML Export");

            // Imposta le opzioni di salvataggio HTML con PageTitle
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.PageTitle = "My Custom Page Title";

            // Salva in HTML con il titolo specificato
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);

            Console.WriteLine("HTML file saved with custom page title: " + outputPath);
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


