---
title: "Enum PdfOptimizationType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Rendering.PdfOptimizationType. Specifica un tipo di ottimizzazione"
type: docs
url: /it/net/aspose.cells.rendering/pdfoptimizationtype/
---
## PdfOptimizationType enumeration

Specifica un tipo di ottimizzazione.

```csharp
public enum PdfOptimizationType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Standard | `0` | Alta qualità di stampa |
| MinimumSize | `1` | La dimensione del file è più importante della qualità di stampa |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PdfOptimizationTypeDemo
    {
        public static void PdfOptimizationTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World");

            // Crea PdfSaveOptions e imposta il tipo di ottimizzazione
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.OptimizationType = PdfOptimizationType.MinimumSize;

            // Salva la cartella di lavoro come PDF con il tipo di ottimizzazione specificato
            workbook.Save("OptimizedOutput.pdf", pdfSaveOptions);

            Console.WriteLine("PDF saved with optimization type: MinimumSize");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


