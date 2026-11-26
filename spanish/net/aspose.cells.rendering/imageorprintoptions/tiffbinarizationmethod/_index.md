---
title: "ImageOrPrintOptions.TiffBinarizationMethod"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. Obtiene o establece el método utilizado al convertir imágenes al formato de 1 bpp cuando ImageType es Tiff y TiffCompression es igual a Ccitt3 o Ccitt4"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/tiffbinarizationmethod/
---
## ImageOrPrintOptions.TiffBinarizationMethod property

Obtiene o establece el método utilizado al convertir imágenes al formato de 1 bpp cuando [`ImageType`](../imagetype/) es Tiff y [`TiffCompression`](../tiffcompression/) es igual a Ccitt3 o Ccitt4.

```csharp
public ImageBinarizationMethod TiffBinarizationMethod { get; set; }
```

### Observaciones

El valor predeterminado es FloydSteinbergDithering.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class ImageOrPrintOptionsPropertyTiffBinarizationMethodDemo
    {
        public static void Run()
        {
            // Crear libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de degradado para la demostración visual
            for (int i = 0; i < 15; i++)
            {
                Cell cell = worksheet.Cells[i, 0];
                cell.PutValue(i * 7);
                Style style = cell.GetStyle();
                style.BackgroundColor = Color.FromArgb(i * 18, i * 18, i * 18);
                cell.SetStyle(style);
            }

            // Configurar opciones de renderizado TIFF
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Tiff,
                TiffCompression = TiffCompression.CompressionCCITT3,
                TiffColorDepth = ColorDepth.Format1bpp
            };

            // Mostrar el método de binarización actual
            Console.WriteLine("Initial TiffBinarizationMethod: " + options.TiffBinarizationMethod);

            // Renderizar con el método de umbral predeterminado
            new SheetRender(worksheet, options).ToImage(0, "ThresholdBinarization.tiff");

            // Cambiar a Floyd-Steinberg dithering
            options.TiffBinarizationMethod = ImageBinarizationMethod.FloydSteinbergDithering;
            Console.WriteLine("\nModified TiffBinarizationMethod: " + options.TiffBinarizationMethod);

            // Renderizar con el nuevo método
            new SheetRender(worksheet, options).ToImage(0, "DitheringBinarization.tiff");

            Console.WriteLine("\nGenerated TIFF files demonstrate different 1bpp conversion methods.");
        }
    }
}
```

### Ver también

* enum [ImageBinarizationMethod](../../imagebinarizationmethod/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


