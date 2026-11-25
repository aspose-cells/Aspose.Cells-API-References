---
title: "PdfSaveOptions.EmbedStandardWindowsFonts"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PdfSaveOptions property. True per incorporare i font TrueType. Influisce solo sui caratteri ASCII 32127. I font per i codici di carattere superiori a 127 sono sempre incorporati. I font sono sempre incorporati per lo standard PDF/A1a PDF/A1b. Il valore predefinito è true"
type: docs
url: /it/net/aspose.cells/pdfsaveoptions/embedstandardwindowsfonts/
---
## PdfSaveOptions.EmbedStandardWindowsFonts property

True per incorporare i caratteri TrueType. Influisce solo sui caratteri ASCII 32-127. I caratteri per codici superiori a 127 sono sempre incorporati. I caratteri sono sempre incorporati per lo standard PDF/A-1a, PDF/A-1b. Il valore predefinito è true.

```csharp
public bool EmbedStandardWindowsFonts { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyEmbedStandardWindowsFontsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test PDF with embedded fonts");

            // Imposta le opzioni di salvataggio PDF con la proprietà EmbedStandardWindowsFonts
            PdfSaveOptions options = new PdfSaveOptions();
            options.EmbedStandardWindowsFonts = true;

            // Salva su stream di memoria
            using (MemoryStream ms = new MemoryStream())
            {
                workbook.Save(ms, options);
                Console.WriteLine("PDF saved with embedded fonts: " + (ms.Length > 0));
            }

            // Dimostra la disattivazione dell'incorporamento dei font
            options.EmbedStandardWindowsFonts = false;
            using (MemoryStream ms = new MemoryStream())
            {
                workbook.Save(ms, options);
                Console.WriteLine("PDF saved without embedded fonts: " + (ms.Length > 0));
            }
        }
    }
}
```

### Vedi anche

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


