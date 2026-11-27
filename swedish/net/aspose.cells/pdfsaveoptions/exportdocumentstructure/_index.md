---
title: "PdfSaveOptions.ExportDocumentStructure"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PdfSaveOptions-egenskap. Anger om dokumentstrukturen ska exporteras"
type: docs
url: /sv/net/aspose.cells/pdfsaveoptions/exportdocumentstructure/
---
## PdfSaveOptions.ExportDocumentStructure property

Anger om dokumentstrukturen ska exporteras.

```csharp
public bool ExportDocumentStructure { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyExportDocumentStructureDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Skapa PDF-sparalternativ
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Ställ in ExportDocumentStructure till true för att behålla dokumentstrukturen
            pdfSaveOptions.ExportDocumentStructure = true;
            
            // Beräkna formler innan sparning
            workbook.CalculateFormula();

            // Spara arbetsboken som PDF med de angivna alternativen
            workbook.Save("output.pdf", pdfSaveOptions);

            Console.WriteLine("PDF saved with document structure exported.");
        }
    }
}
```

### Se även

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


