---
title: "PdfSaveOptions.OptimizationType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PdfSaveOptions‑Eigenschaft. Ruft den PDF‑Optimierungstyp ab und legt ihn fest"
type: docs
url: /de/net/aspose.cells/pdfsaveoptions/optimizationtype/
---
## PdfSaveOptions.OptimizationType property

Liest und setzt den PDF-Optimierungstyp.

```csharp
public PdfOptimizationType OptimizationType { get; set; }
```

### Hinweise

Der Standardwert ist Standard

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells PDF Optimization Example");

            // PDF-Speicheroptionen erstellen
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Demonstration der OptimizationType‑Eigenschaft
            pdfSaveOptions.OptimizationType = PdfOptimizationType.MinimumSize;

            // Speichern Sie die Arbeitsmappe mit Optimierungseinstellungen
            workbook.Save("OptimizedPdf.pdf", pdfSaveOptions);
        }
    }
}
```

### Siehe auch

* enum [PdfOptimizationType](../../../aspose.cells.rendering/pdfoptimizationtype/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


