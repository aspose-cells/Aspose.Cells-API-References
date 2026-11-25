---
title: "Enum PrintingPageType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.PrintingPageType enum. Indica quali pagine non verranno stampate"
type: docs
url: /it/net/aspose.cells/printingpagetype/
---
## PrintingPageType enumeration

Indica quali pagine non saranno stampate.

```csharp
public enum PrintingPageType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Default | `0` | Stampa tutte le pagine. |
| IgnoreBlank | `1` | Non stampare le pagine in cui le celle sono vuote. |
| IgnoreStyle | `2` | Non stampare le pagine in cui le celle contengono solo stili. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PrintingPageTypeDemo
    {
        public static void PrintingPageTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Inserisci alcuni dati nel foglio di lavoro
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");
            worksheet.Cells["A3"].PutValue("!");

            // Crea PdfSaveOptions
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Imposta PrintingPageType su IgnoreBlank
            pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreBlank;

            // Salva la cartella di lavoro in PDF con le opzioni specificate
            workbook.Save("output_ignore_blank_page.pdf", pdfSaveOptions);

            // Imposta PrintingPageType su IgnoreStyle
            pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreStyle;

            // Salva la cartella di lavoro in PDF con le opzioni specificate
            workbook.Save("output_ignore_blank_and_style_page.pdf", pdfSaveOptions);

            // Imposta PrintingPageType su Default
            pdfSaveOptions.PrintingPageType = PrintingPageType.Default;

            // Salva la cartella di lavoro in PDF con le opzioni specificate
            workbook.Save("output_default_page.pdf", pdfSaveOptions);

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


