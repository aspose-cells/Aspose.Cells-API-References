---
title: "PageSavingArgs.PageIndex"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSavingArgs. Índice de página actual basado en cero"
type: docs
url: /es/net/aspose.cells.rendering/pagesavingargs/pageindex/
---
## PageSavingArgs.PageIndex property

Índice de página actual, basado en cero.

```csharp
public int PageIndex { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PageSavingArgsPropertyPageIndexDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunos datos a la hoja de cálculo
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data row {i + 1}";
            }

            // Crea opciones de guardado PDF
            PdfSaveOptions options = new PdfSaveOptions();
            
            // Establecer la devolución de llamada de guardado de página
            options.PageSavingCallback = new PageSavingCallback();

            // Guardar el libro de trabajo en PDF - esto activará la devolución de llamada para cada página
            workbook.Save("output.pdf", options);
        }
    }

    public class PageSavingCallback : IPageSavingCallback
    {
        public void PageStartSaving(PageStartSavingArgs args)
        {
            // Demostrar el uso de la propiedad PageIndex
            Console.WriteLine($"Starting to save page {args.PageIndex + 1}");
        }

        public void PageEndSaving(PageEndSavingArgs args)
        {
            // No se usa en este ejemplo
        }
    }
}
```

### Ver también

* class [PageSavingArgs](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


