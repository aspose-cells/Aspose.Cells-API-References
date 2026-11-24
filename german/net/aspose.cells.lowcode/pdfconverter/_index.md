---
title: "Klasse PdfConverter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.LowCode.PdfConverter Klasse. Konverter zum Konvertieren von Vorlagendateien in PDF"
type: docs
url: /de/net/aspose.cells.lowcode/pdfconverter/
---
## PdfConverter class

Konverter zum Konvertieren von Vorlagendateien in PDF.

```csharp
public class PdfConverter
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/pdfconverter/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions) | Konvertiert Vorlagendateien in PDF |
| static [Process](../../aspose.cells.lowcode/pdfconverter/process/#process_1)(string, string) | Konvertiert die angegebene Vorlagendatei in PDF. |

### Beispiele

```csharp
using System;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassPdfConverterDemo
    {
        public static void Run()
        {
            // Initialisieren Sie den PdfConverter mit Vorlage- und Ausgabepfaden
            PdfConverter.Process("template.xlsx", "res.pdf");
            
            Console.WriteLine("PDF conversion completed successfully.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


