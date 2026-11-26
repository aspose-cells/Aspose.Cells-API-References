---
title: "ImageOrPrintOptions.PageIndex"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. Obtiene o establece el índice basado en 0 de la primera página a guardar"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/pageindex/
---
## ImageOrPrintOptions.PageIndex property

Obtiene o establece el índice basado en cero de la primera página a guardar.

```csharp
public int PageIndex { get; set; }
```

### Observaciones

El valor predeterminado es 0.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyPageIndexDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a varias páginas
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Data Row " + (i + 1);
            }

            // Configurar opciones de imagen/impresión
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PageIndex = 1; // Start from second page (0-based index would be 1)
            options.PageCount = 1; // Only process one page

            // Crear renderizado de hoja para la primera hoja de cálculo
            SheetRender render = new SheetRender(worksheet, options);

            // Guardar en PDF usando el método API correcto
            render.ToImage(0, "output.pdf");
            Console.WriteLine("Saved page 2 to PDF successfully.");
        }
    }
}
```

### Ver también

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


