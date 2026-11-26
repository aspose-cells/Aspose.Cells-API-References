---
title: "Clase PageSavingArgs"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Rendering.PageSavingArgs. Información sobre un proceso de guardado de página"
type: docs
url: /es/net/aspose.cells.rendering/pagesavingargs/
---
## PageSavingArgs class

Información para el proceso de guardado de una página.

```csharp
public class PageSavingArgs
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [PageCount](../../aspose.cells.rendering/pagesavingargs/pagecount/) { get; } | Recuento total de páginas. |
| [PageIndex](../../aspose.cells.rendering/pagesavingargs/pageindex/) { get; } | Índice de página actual, basado en cero. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassPageSavingArgsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con datos extendidos para múltiples páginas
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Poblar la hoja de cálculo para generar múltiples páginas al renderizarse
            for (int row = 0; row < 150; row++)
            {
                worksheet.Cells[row, 0].Value = $"Row {row + 1} data";
            }

            // Configurar opciones de guardado PDF con devolución de llamada de guardado de página
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.PageSavingCallback = new PageSavingCallback();

            // Guardar el libro de trabajo en formato PDF con paginación
            workbook.Save("RenderingPageSavingDemo.pdf", pdfSaveOptions);
        }

        private class PageSavingCallback : IPageSavingCallback
        {
            public void PageStartSaving(PageStartSavingArgs args)
            {
                Console.WriteLine($"Saving page {args.PageIndex + 1} of {args.PageCount}");
                
                if (args.PageIndex == 0)
                {
                    Console.WriteLine("Processing cover page...");
                }
            }

            public void PageEndSaving(PageEndSavingArgs args)
            {
                // Opcional: Añadir cualquier procesamiento de fin de página aquí
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


