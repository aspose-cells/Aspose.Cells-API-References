---
title: "ImageOrPrintOptions.IsOptimized"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. Indica si se deben optimizar los elementos de salida"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/isoptimized/
---
## ImageOrPrintOptions.IsOptimized property

Indica si se deben optimizar los elementos de salida.

```csharp
public bool IsOptimized { get; set; }
```

### Observaciones

El valor predeterminado es false. Actualmente, cuando esta propiedad se establece en true, se realizarán las siguientes optimizaciones: 1. optimizar las líneas de borde. 2. optimizar el tamaño del archivo al renderizar a imagen Svg.

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyIsOptimizedDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a las celdas
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    sheet.Cells[i, j].PutValue($"Data {i}-{j}");
                }
            }

            // Configurar opciones de renderizado de imagen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.OnePagePerSheet = true;
            
            // Demostrar la propiedad IsOptimized
            options.IsOptimized = true; // Enable optimization
            
            // Renderizar la hoja a imagen
            SheetRender renderer = new SheetRender(sheet, options);
            MemoryStream stream = new MemoryStream();
            renderer.ToImage(0, stream);
            
            Console.WriteLine($"Image rendered with optimization: {options.IsOptimized}");
            Console.WriteLine($"Image size: {stream.Length} bytes");
        }
    }
}
```

### Ver también

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


