---
title: "Enum PdfOptimizationType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.Rendering.PdfOptimizationType. Especifica un tipo de optimización."
type: docs
url: /es/net/aspose.cells.rendering/pdfoptimizationtype/
---
## PdfOptimizationType enumeration

Especifica un tipo de optimización.

```csharp
public enum PdfOptimizationType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Standard | `0` | Alta calidad de impresión |
| MinimumSize | `1` | El tamaño del archivo es más importante que la calidad de impresión |

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World");

            // Crea PdfSaveOptions y establece el tipo de optimización
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.OptimizationType = PdfOptimizationType.MinimumSize;

            // Guarda el libro de trabajo como PDF con el tipo de optimización especificado
            workbook.Save("OptimizedOutput.pdf", pdfSaveOptions);

            Console.WriteLine("PDF saved with optimization type: MinimumSize");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


