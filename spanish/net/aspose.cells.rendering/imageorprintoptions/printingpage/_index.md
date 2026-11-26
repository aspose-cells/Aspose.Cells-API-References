---
title: "ImageOrPrintOptions.PrintingPage"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. Indica qué páginas no se imprimirán"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/printingpage/
---
## ImageOrPrintOptions.PrintingPage property

Indica qué páginas no se imprimirán.

```csharp
public PrintingPageType PrintingPage { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyPrintingPageDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunos datos a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Test Data");
            worksheet.Cells["A2"].PutValue("Non-Blank Cell");
            worksheet.Cells["A5"].PutValue("Another Non-Blank Cell");
            
            // Crear opciones de imagen/impresión
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PrintingPage = PrintingPageType.IgnoreBlank;
            
            // Renderizar el libro de trabajo con las opciones
            WorkbookRender render = new WorkbookRender(workbook, options);
            
            // Salida del recuento de páginas (ignora las páginas en blanco)
            Console.WriteLine("Page count with IgnoreBlank: " + render.PageCount);
            
            // Cambiar al comportamiento predeterminado (incluir todas las páginas)
            options.PrintingPage = PrintingPageType.Default;
            render = new WorkbookRender(workbook, options);
            Console.WriteLine("Page count with Default: " + render.PageCount);
        }
    }
}
```

### Ver también

* enum [PrintingPageType](../../../aspose.cells/printingpagetype/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


