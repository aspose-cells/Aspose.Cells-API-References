---
title: "WorkbookPrintingPreview.EvaluatedPageCount"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookPrintingPreview. Evalúa el recuento total de páginas de este libro de trabajo"
type: docs
url: /es/net/aspose.cells.rendering/workbookprintingpreview/evaluatedpagecount/
---
## WorkbookPrintingPreview.EvaluatedPageCount property

Evaluar el recuento total de páginas de este libro de trabajo

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
    public class WorkbookPrintingPreviewPropertyEvaluatedPageCountDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo a la hoja de cálculo
            for (int i = 0; i < 100; i++)
            {
                worksheet.Cells[i, 0].PutValue("Row " + (i + 1));
            }

            // Crear opciones de vista previa de impresión
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // Crear vista previa de impresión del libro de trabajo
            WorkbookPrintingPreview printingPreview = new WorkbookPrintingPreview(workbook, options);
            
            // Obtener y mostrar el recuento de páginas evaluado
            Console.WriteLine("Evaluated Page Count: " + printingPreview.EvaluatedPageCount);
        }
    }
}
```

### Ver también

* class [WorkbookPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


