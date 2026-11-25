---
title: "Classe PdfConverter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.LowCode.PdfConverter. Convertitore per trasformare il file modello in PDF"
type: docs
url: /it/net/aspose.cells.lowcode/pdfconverter/
---
## PdfConverter class

Convertitore per la conversione di file modello in PDF.

```csharp
public class PdfConverter
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/pdfconverter/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions) | Converte il file modello in PDF |
| static [Process](../../aspose.cells.lowcode/pdfconverter/process/#process_1)(string, string) | Converte il file modello fornito in PDF. |

### Esempi

```csharp
using System;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassPdfConverterDemo
    {
        public static void Run()
        {
            // Inizializza il PdfConverter con i percorsi del modello e dell'output
            PdfConverter.Process("template.xlsx", "res.pdf");
            
            Console.WriteLine("PDF conversion completed successfully.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


