---
title: "Enum PdfOptimizationType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Rendering.PdfOptimizationType enum. Anger en typ av optimering"
type: docs
url: /sv/net/aspose.cells.rendering/pdfoptimizationtype/
---
## PdfOptimizationType enumeration

Anger en typ av optimering.

```csharp
public enum PdfOptimizationType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Standard | `0` | Hög utskriftskvalitet |
| MinimumSize | `1` | Filstorlek är viktigare än utskriftskvalitet |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World");

            // Skapa PdfSaveOptions och ange optimeringstypen
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.OptimizationType = PdfOptimizationType.MinimumSize;

            // Spara arbetsboken som en PDF med den angivna optimeringstypen
            workbook.Save("OptimizedOutput.pdf", pdfSaveOptions);

            Console.WriteLine("PDF saved with optimization type: MinimumSize");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


