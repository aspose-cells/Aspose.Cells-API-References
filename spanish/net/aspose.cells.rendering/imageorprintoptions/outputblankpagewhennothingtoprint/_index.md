---
title: "ImageOrPrintOptions.OutputBlankPageWhenNothingToPrint"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. Indica si se debe generar una página en blanco cuando no hay nada que imprimir"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/outputblankpagewhennothingtoprint/
---
## ImageOrPrintOptions.OutputBlankPageWhenNothingToPrint property

Indica si se debe generar una página en blanco cuando no hay nada que imprimir.

```csharp
public bool OutputBlankPageWhenNothingToPrint { get; set; }
```

### Observaciones

El valor predeterminado es falso.

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyOutputBlankPageWhenNothingToPrintDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo vacío
            Workbook workbook = new Workbook();
            
            // Accede a la primera hoja de cálculo que está vacía
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer opciones de imagen o impresión
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.OnePagePerSheet = true;
            
            // Demuestra la propiedad OutputBlankPageWhenNothingToPrint
            options.OutputBlankPageWhenNothingToPrint = true;
            
            // Renderiza la hoja
            SheetRender renderer = new SheetRender(worksheet, options);
            
            // La salida seguirá produciendo una página en blanco debido a la configuración de la propiedad
            Console.WriteLine("Page count with OutputBlankPageWhenNothingToPrint=true: " + renderer.PageCount);
            
            // Guarda la primera página en un flujo de memoria
            MemoryStream stream = new MemoryStream();
            renderer.ToImage(0, stream);
            Console.WriteLine("Image data length: " + stream.ToArray().Length);
            
            // Ahora establece la propiedad en falso
            options.OutputBlankPageWhenNothingToPrint = false;
            SheetRender renderer2 = new SheetRender(worksheet, options);
            
            // La salida tendrá cero páginas ahora
            Console.WriteLine("Page count with OutputBlankPageWhenNothingToPrint=false: " + renderer2.PageCount);
        }
    }
}
```

### Ver también

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


