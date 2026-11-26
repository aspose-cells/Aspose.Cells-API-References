---
title: "Range.ToImage"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Range. Convierte el rango a una imagen"
type: docs
url: /es/net/aspose.cells/range/toimage/
---
## Range.ToImage method

Convierte el rango a imagen.

```csharp
public byte[] ToImage(ImageOrPrintOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| opciones | ImageOrPrintOptions | Las opciones para convertir este rango a una imagen |

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RangeMethodToImageWithImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Cree un libro de trabajo a partir de un archivo Excel de ejemplo
            Workbook workbook = new Workbook("example.xlsx");
            
            // Obtenga la primera hoja y sus celdas
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Cree el rango A1:J25
            Aspose.Cells.Range range = cells.CreateRange("A1:J25");
            
            // Crear opciones de imagen
            ImageOrPrintOptions options = new ImageOrPrintOptions()
            {
                ImageType = Aspose.Cells.Drawing.ImageType.Png,
                HorizontalResolution = 300,
                VerticalResolution = 300
            };
            
            // Convertir el rango a una imagen
            byte[] imageData = range.ToImage(options);
            
            // Guardar la imagen en un archivo
            File.WriteAllBytes("range_output.png", imageData);
        }
    }
}
```

### Ver también

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


