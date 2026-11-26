---
title: "PageSavingArgs.PageCount"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSavingArgs. Recuento total de páginas"
type: docs
url: /es/net/aspose.cells.rendering/pagesavingargs/pagecount/
---
## PageSavingArgs.PageCount property

Recuento total de páginas.

```csharp
public int PageCount { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PageSavingArgsPropertyPageCountDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo y añada datos de prueba
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar contenido denso para crear múltiples páginas
            for (int i = 0; i < 500; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }

            // Configurar la configuración de página para controlar la paginación
            worksheet.PageSetup.PrintArea = "A1:A50";
            worksheet.PageSetup.PaperSize = PaperSizeType.PaperLetter;

            // Crear opciones de guardado de PDF con la devolución de llamada de guardado de página
            PdfSaveOptions options = new PdfSaveOptions();
            options.PageSavingCallback = new PageSavingCallback();

            // Guardar a PDF para activar la paginación
            workbook.Save("PageSavingDemo.pdf", options);
        }

        private class PageSavingCallback : IPageSavingCallback
        {
            public void PageStartSaving(PageStartSavingArgs args)
            {
                // Acceder a PageCount desde los argumentos del evento
                Console.WriteLine($"Saving page {args.PageIndex + 1} of {args.PageCount}");
            }

            public void PageEndSaving(PageEndSavingArgs args)
            {
                // No se necesita implementación
            }
        }
    }
}
```

### Ver también

* class [PageSavingArgs](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


