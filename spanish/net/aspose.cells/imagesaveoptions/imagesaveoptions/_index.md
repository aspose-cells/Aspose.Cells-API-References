---
title: "ImageSaveOptions.ImageSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor ImageSaveOptions. Crea las opciones para guardar un archivo de imagen"
type: docs
url: /es/net/aspose.cells/imagesaveoptions/imagesaveoptions/
---
## ImageSaveOptions() {#constructor}

Crea las opciones para guardar el archivo de imagen.

```csharp
public ImageSaveOptions()
```

### Observaciones

El tipo predeterminado es Tiff.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ImageSaveOptionsMethodSharpctorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos para contexto
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Demostrar el constructor sin parámetros
                ImageSaveOptions defaultOptions = new ImageSaveOptions();
                Console.WriteLine("Created ImageSaveOptions with default constructor");

                // Demostrar el constructor con el parámetro SaveFormat
                ImageSaveOptions pngOptions = new ImageSaveOptions(SaveFormat.Png);
                Console.WriteLine("Created ImageSaveOptions with SaveFormat.Png");

                // Acceder a la propiedad de solo lectura ImageOrPrintOptions
                var imageOptions = pngOptions.ImageOrPrintOptions;
                Console.WriteLine($"ImageOrPrintOptions type: {imageOptions.GetType().Name}");

                // Establecer la propiedad StreamProvider
                pngOptions.StreamProvider = null;
                Console.WriteLine("StreamProvider set to null");

                // Guardar el libro de trabajo con las opciones creadas
                workbook.Save("output.png", pngOptions);
                Console.WriteLine("Workbook saved successfully with ImageSaveOptions");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [ImageSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImageSaveOptions(SaveFormat) {#constructor_1}

Crea las opciones para guardar el archivo de imagen.

```csharp
public ImageSaveOptions(SaveFormat saveFormat)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| saveFormat | SaveFormat | El formato de archivo. Debe ser uno de los siguientes tipos: Tiff, Svg, Bmp, Png, Jpg, Emf o Gif, de lo contrario el formato guardado se establecerá automáticamente como Tiff. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo y añada datos de prueba
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells Image Save Demo");
            
            // Cree ImageSaveOptions con SaveFormat.Tiff
            try
            {
                ImageSaveOptions saveOptions = new ImageSaveOptions(SaveFormat.Tiff);
                
                // Configurar opciones de renderizado de imagen
                saveOptions.ImageOrPrintOptions.HorizontalResolution = 300;
                saveOptions.ImageOrPrintOptions.VerticalResolution = 300;

                // Guarde el libro de trabajo como TIFF multipágina
                workbook.Save("WorksheetImage.tiff", saveOptions);
                
                Console.WriteLine("Workbook successfully saved as TIFF image with 300 DPI resolution.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during image save operation: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* enum [SaveFormat](../../saveformat/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


