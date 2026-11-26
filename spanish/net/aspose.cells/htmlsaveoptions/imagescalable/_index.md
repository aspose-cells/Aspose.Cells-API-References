---
title: "HtmlSaveOptions.ImageScalable"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si se usa una unidad escalable para describir el ancho de la imagen al usar una unidad escalable para describir el ancho de la columna. El valor predeterminado es verdadero"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/imagescalable/
---
## HtmlSaveOptions.ImageScalable property

Indica si se utiliza una unidad escalable para describir el ancho de la imagen al usar una unidad escalable para describir el ancho de la columna. El valor predeterminado es true.

```csharp
public bool ImageScalable { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyImageScalableDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de ejemplo con una imagen
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar una imagen de ejemplo a la hoja de cálculo
            int imgIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[imgIndex];

            // Establecer opciones de guardado HTML con la propiedad ImageScalable
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ImageScalable = false; // Images won't scale with the HTML content
            
            // Guarda el libro de trabajo como HTML
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML file saved with ImageScalable set to false.");
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


