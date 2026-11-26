---
title: "WorkbookRender.PageCount"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookRender. Obtiene el recuento total de páginas del libro de trabajo"
type: docs
url: /es/net/aspose.cells.rendering/workbookrender/pagecount/
---
## WorkbookRender.PageCount property

Obtiene el recuento total de páginas del libro de trabajo.

```csharp
public int PageCount { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookRenderPropertyPageCountDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Page 1 Content");
            
            // Agregar una segunda hoja de cálculo
            workbook.Worksheets.Add();
            worksheet = workbook.Worksheets[1];
            worksheet.Cells["A1"].PutValue("Page 2 Content");

            // Crear opciones de renderizado y renderizador de libro de trabajo
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                OnePagePerSheet = true
            };
            
            WorkbookRender renderer = new WorkbookRender(workbook, options);

            // Demostrar el uso de PageCount
            Console.WriteLine($"Total pages to render: {renderer.PageCount}");
            
            // Renderizar cada página a imagen
            for (int i = 0; i < renderer.PageCount; i++)
            {
                string outputPath = $"Page_{i}.png";
                renderer.ToImage(i, outputPath);
                Console.WriteLine($"Rendered page {i+1} to {outputPath}");
            }
        }
    }
}
```

### Ver también

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


