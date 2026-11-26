---
title: "PaginatedSaveOptions.PageSavingCallback"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PaginatedSaveOptions. Controla/Indica el progreso del proceso de guardado de páginas"
type: docs
url: /es/net/aspose.cells/paginatedsaveoptions/pagesavingcallback/
---
## PaginatedSaveOptions.PageSavingCallback property

Controlar/Indicar el progreso del proceso de guardado de la página.

```csharp
public IPageSavingCallback PageSavingCallback { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyPageSavingCallbackDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Page 1 Content");
            worksheet.Cells["A2"].PutValue("This demonstrates PageSavingCallback");

            // Cree opciones de guardado con devolución de llamada de guardado de página
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.PageSavingCallback = new CustomPageSavingCallback();

            // Guardar con devolución de llamada
            workbook.Save("PageSavingCallbackDemo.pdf", saveOptions);
        }
    }

    public class CustomPageSavingCallback : IPageSavingCallback
    {
        public void PageStartSaving(PageStartSavingArgs args)
        {
            Console.WriteLine($"Starting to save page {args.PageIndex + 1}");
        }

        public void PageEndSaving(PageEndSavingArgs args)
        {
            Console.WriteLine($"Finished saving page {args.PageIndex + 1}");
            if (args.HasMorePages)
            {
                Console.WriteLine("More pages to follow...");
            }
        }
    }
}
```

### Ver también

* interface [IPageSavingCallback](../../../aspose.cells.rendering/ipagesavingcallback/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


