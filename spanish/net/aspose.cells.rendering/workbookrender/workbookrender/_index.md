---
title: "WorkbookRender.WorkbookRender"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor WorkbookRender. La construcción de WorkbookRender"
type: docs
url: /es/net/aspose.cells.rendering/workbookrender/workbookrender/
---
## WorkbookRender constructor

La construcción de WorkbookRender

```csharp
public WorkbookRender(Workbook workbook, ImageOrPrintOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| libro de trabajo | Libro de trabajo | Indicar qué libro de trabajo será renderizado. |
| opciones | ImageOrPrintOptions | ImageOrPrintOptions contiene algunas propiedades de la imagen de salida |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookRenderMethodctorWithWorkbookImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            
            // Crear opciones de imagen/impresión
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // Crear renderizador de libro de trabajo
            WorkbookRender renderer = new WorkbookRender(workbook, options);
            
            // Salida del recuento de páginas
            Console.WriteLine("Total pages: " + renderer.PageCount);
        }
    }
}
```

### Ver también

* class [Workbook](../../../aspose.cells/workbook/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


