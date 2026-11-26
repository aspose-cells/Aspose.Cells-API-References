---
title: "Enum ImageBinarizationMethod"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.Rendering.ImageBinarizationMethod. Especifica el método utilizado para binarizar la imagen"
type: docs
url: /es/net/aspose.cells.rendering/imagebinarizationmethod/
---
## ImageBinarizationMethod enumeration

Especifica el método utilizado para binarizar la imagen.

```csharp
public enum ImageBinarizationMethod
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Threshold | `0` | Especifica el método de umbral. |
| FloydSteinbergDithering | `1` | Especifica el tramado usando el método de difusión de error Floyd‑Steinberg. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class RenderingClassImageBinarizationMethodDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con datos de prueba
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Rellenar celdas con valores de degradado para demostración
            for (int row = 0; row < 50; row++)
            {
                for (int col = 0; col < 10; col++)
                {
                    worksheet.Cells[row, col].PutValue((double)(row * col) / 500);
                }
            }

            // Configurar opciones de renderizado de imagen
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Tiff,
                TiffCompression = TiffCompression.CompressionCCITT4,
                TiffBinarizationMethod = ImageBinarizationMethod.FloydSteinbergDithering
            };

            // Crear renderizado de hoja con opciones configuradas
            SheetRender renderer = new SheetRender(worksheet, options);
            
            // Renderizar la primera página de la hoja de cálculo a imagen con binarización
            renderer.ToImage(0, "BinarizedOutput.tiff");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


