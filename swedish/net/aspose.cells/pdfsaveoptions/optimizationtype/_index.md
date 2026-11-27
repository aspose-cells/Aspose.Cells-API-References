---
title: "PdfSaveOptions.OptimizationType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PdfSaveOptions-egenskap. Hämtar och anger pdf-optimeringstyp"
type: docs
url: /sv/net/aspose.cells/pdfsaveoptions/optimizationtype/
---
## PdfSaveOptions.OptimizationType property

Hämtar och anger pdf‑optimeringstyp.

```csharp
public PdfOptimizationType OptimizationType { get; set; }
```

### Anmärkningar

Standardvärdet är Standard

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyOptimizationTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells PDF Optimization Example");

            // Skapa PDF-sparalternativ
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Demonstrera OptimizationType-egenskapen
            pdfSaveOptions.OptimizationType = PdfOptimizationType.MinimumSize;

            // Spara arbetsboken med optimeringsinställningar
            workbook.Save("OptimizedPdf.pdf", pdfSaveOptions);
        }
    }
}
```

### Se även

* enum [PdfOptimizationType](../../../aspose.cells.rendering/pdfoptimizationtype/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


