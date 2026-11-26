---
title: "SheetPrintingPreview.EvaluatedPageCount"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SheetPrintingPreview. Evalúa el recuento total de páginas de esta hoja de cálculo"
type: docs
url: /es/net/aspose.cells.rendering/sheetprintingpreview/evaluatedpagecount/
---
## SheetPrintingPreview.EvaluatedPageCount property

Evalúe el recuento total de páginas de esta hoja de cálculo

```csharp
public int EvaluatedPageCount { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetPrintingPreviewPropertyEvaluatedPageCountDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo a la hoja de cálculo
            for (int i = 0; i < 100; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }

            ImageOrPrintOptions options = new ImageOrPrintOptions();
            SheetPrintingPreview preview = new SheetPrintingPreview(worksheet, options);
            
            Console.WriteLine("Evaluated Page Count: " + preview.EvaluatedPageCount);
        }
    }
}
```

### Ver también

* class [SheetPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


