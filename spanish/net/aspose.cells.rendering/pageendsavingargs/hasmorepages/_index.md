---
title: "PageEndSavingArgs.HasMorePages"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageEndSavingArgs. Obtiene o establece un valor que indica si hay más páginas para generar. El valor predeterminado es true"
type: docs
url: /es/net/aspose.cells.rendering/pageendsavingargs/hasmorepages/
---
## PageEndSavingArgs.HasMorePages property

Obtiene o establece un valor que indica si hay más páginas para generar. El valor predeterminado es true.

```csharp
public bool HasMorePages { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PageEndSavingArgsPropertyHasMorePagesDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos que abarcan varias páginas
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 500; i++)
            {
                worksheet.Cells[i, 0].Value = $"Row {i + 1}";
            }

            // Crear opciones de guardado PDF con manejo de página personalizado
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.PageSavingCallback = new PageControlCallback();

            // Guardar el libro de trabajo con limitación de páginas
            workbook.Save("PropertyHasMorePagesDemo.pdf", saveOptions);
        }
    }

    internal class PageControlCallback : IPageSavingCallback
    {
        private int pageCount = 0;

        public void PageStartSaving(PageStartSavingArgs args)
        {
            // No se usa en esta demostración
        }

        public void PageEndSaving(PageEndSavingArgs args)
        {
            // Leer el valor actual de la propiedad
            Console.WriteLine($"Page {pageCount} - Initial HasMorePages: {args.HasMorePages}");

            // Modificar la propiedad después de la primera página
            if (pageCount == 0)
            {
                args.HasMorePages = false;
                Console.WriteLine($"Page {pageCount} - Updated HasMorePages: {args.HasMorePages}");
            }

            pageCount++;
        }
    }
}
```

### Ver también

* class [PageEndSavingArgs](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


