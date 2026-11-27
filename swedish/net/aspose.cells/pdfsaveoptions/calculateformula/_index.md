---
title: "PdfSaveOptions.CalculateFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PdfSaveOptions egenskap. Anger om formler ska beräknas innan PDF-filen sparas"
type: docs
url: /sv/net/aspose.cells/pdfsaveoptions/calculateformula/
---
## PdfSaveOptions.CalculateFormula property

Anger om formler ska beräknas innan pdf‑filen sparas.

```csharp
public bool CalculateFormula { get; set; }
```

### Anmärkningar

Standardvärdet är falskt.

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyCalculateFormulaDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata och formler
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ange värden och formler
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // Skapa PDF-sparalternativ med formelberäkning
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.CalculateFormula = true;

            // Spara till minnesström
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, pdfSaveOptions);
                
                // Återställ strömmens position och verifiera innehållet
                stream.Position = 0;
                using (StreamReader reader = new StreamReader(stream))
                {
                    string content = reader.ReadToEnd();
                    Console.WriteLine("PDF contains formula results: " + content.Contains("30"));
                }
            }
        }
    }
}
```

### Se även

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


