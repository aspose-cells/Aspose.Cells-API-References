---
title: "Clase PageStartSavingArgs"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Rendering.PageStartSavingArgs. Información para el inicio del proceso de guardado de una página"
type: docs
url: /es/net/aspose.cells.rendering/pagestartsavingargs/
---
## PageStartSavingArgs class

Información para el proceso de inicio de guardado de una página.

```csharp
public class PageStartSavingArgs : PageSavingArgs
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [IsToOutput](../../aspose.cells.rendering/pagestartsavingargs/istooutput/) { get; set; } | Obtiene o establece un valor que indica si la página debe ser exportada. El valor predeterminado es true. |
| [PageCount](../../aspose.cells.rendering/pagesavingargs/pagecount/) { get; } | Recuento total de páginas.(Her​edado de [`PageSavingArgs`](../pagesavingargs/).) |
| [PageIndex](../../aspose.cells.rendering/pagesavingargs/pageindex/) { get; } | Índice de página actual, basado en cero.(Her​edado de [`PageSavingArgs`](../pagesavingargs/).) |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingClassPageStartSavingArgsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].PutValue("Hello World");
            
            PdfSaveOptions options = new PdfSaveOptions();
            options.PageSavingCallback = new CustomPageSavingCallback();
            
            workbook.Save("output.pdf", options);
        }
    }
    
    public class CustomPageSavingCallback : IPageSavingCallback
    {
        public void PageStartSaving(PageStartSavingArgs args)
        {
            Console.WriteLine($"Starting to save page {args.PageIndex}");
        }
        
        public void PageEndSaving(PageEndSavingArgs args)
        {
            // Implementación opcional
        }
    }
}
```

### Ver también

* class [PageSavingArgs](../pagesavingargs/)
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


