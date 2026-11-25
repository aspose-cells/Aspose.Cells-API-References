---
title: "PdfSaveOptions.OptimizationType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PdfSaveOptions. Ottiene e imposta il tipo di ottimizzazione pdf"
type: docs
url: /it/net/aspose.cells/pdfsaveoptions/optimizationtype/
---
## PdfSaveOptions.OptimizationType property

Ottiene e imposta il tipo di ottimizzazione pdf.

```csharp
public PdfOptimizationType OptimizationType { get; set; }
```

### Osservazioni

Il valore predefinito è Standard

### Esempi

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
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells PDF Optimization Example");

            // Crea le opzioni di salvataggio PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Dimostra la proprietà OptimizationType
            pdfSaveOptions.OptimizationType = PdfOptimizationType.MinimumSize;

            // Salva la cartella di lavoro con le impostazioni di ottimizzazione
            workbook.Save("OptimizedPdf.pdf", pdfSaveOptions);
        }
    }
}
```

### Vedi anche

* enum [PdfOptimizationType](../../../aspose.cells.rendering/pdfoptimizationtype/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


