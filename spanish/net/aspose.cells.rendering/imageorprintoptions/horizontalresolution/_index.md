---
title: "ImageOrPrintOptions.HorizontalResolution"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. Obtiene o establece la resolución horizontal para imágenes generadas en puntos por pulgada"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/horizontalresolution/
---
## ImageOrPrintOptions.HorizontalResolution property

Obtiene o establece la resolución horizontal para las imágenes generadas, en puntos por pulgada.

```csharp
public int HorizontalResolution { get; set; }
```

### Observaciones

El valor predeterminado es 96.

Configurar `HorizontalResolution` y [`VerticalResolution`](../verticalresolution/) afecta el ancho y la altura de la imagen de salida en píxeles.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyHorizontalResolutionDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Text for Image Rendering");

            // Inicializar ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Png;
            
            // Establecer resolución horizontal y vertical
            options.HorizontalResolution = 192;
            options.VerticalResolution = 192;

            // Renderizar la hoja de cálculo a imagen con la resolución especificada
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "WorksheetImage_192dpi.png");

            // Demostrar diferentes resoluciones
            options.HorizontalResolution = 300;
            options.VerticalResolution = 300;
            renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "WorksheetImage_300dpi.png");
        }
    }
}
```

### Ver también

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


