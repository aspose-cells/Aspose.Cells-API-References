---
title: "Clase PageEndSavingArgs"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Rendering.PageEndSavingArgs. Información para el proceso de finalización del guardado de una página"
type: docs
url: /es/net/aspose.cells.rendering/pageendsavingargs/
---
## PageEndSavingArgs class

La información de una página finaliza el proceso de guardado.

```csharp
public class PageEndSavingArgs : PageSavingArgs
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [HasMorePages](../../aspose.cells.rendering/pageendsavingargs/hasmorepages/) { get; set; } | Obtiene o establece un valor que indica si hay más páginas para generar. El valor predeterminado es true. |
| [PageCount](../../aspose.cells.rendering/pagesavingargs/pagecount/) { get; } | Recuento total de páginas.(Her​edado de [`PageSavingArgs`](../pagesavingargs/).) |
| [PageIndex](../../aspose.cells.rendering/pagesavingargs/pageindex/) { get; } | Índice de página actual, basado en cero.(Her​edado de [`PageSavingArgs`](../pagesavingargs/).) |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingClassPageEndSavingArgsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Crea una instancia de PdfSaveOptions
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Establecer la devolución de llamada PageEndSaving
            saveOptions.PageSavingCallback = new PageEndSavingArgsTest();

            // Guardar el libro de trabajo con la devolución de llamada
            workbook.Save("output.pdf", saveOptions);
        }
    }

    public class PageEndSavingArgsTest : IPageSavingCallback
    {
        public void PageEndSaving(PageEndSavingArgs args)
        {
            Console.WriteLine($"Finished saving page {args.PageIndex}");
        }

        public void PageStartSaving(PageStartSavingArgs args)
        {
            // Implementación no necesaria para esta demostración
        }
    }
}
```

### Ver también

* class [PageSavingArgs](../pagesavingargs/)
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


