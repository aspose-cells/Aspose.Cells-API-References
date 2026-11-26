---
title: "MsoFillFormatHelper.ImageData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "MsoFillFormatHelper property. Obtiene y establece los datos de relleno de Texture y Picture"
type: docs
url: /es/net/aspose.cells.drawing/msofillformathelper/imagedata/
---
## MsoFillFormatHelper.ImageData property

Obtiene y establece los datos de relleno de textura y de imagen.

```csharp
public byte[] ImageData { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;
    using System.IO;

    public class MsoFillFormatHelperPropertyImageDataDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una etiqueta para que el ejemplo sea significativo
            worksheet.Cells["A1"].Value = "ImageData Property Demo";

            try
            {
                // Crear una instancia de MsoFillFormatHelper usando reflexión (sin constructor público)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Muestra el valor actual de la propiedad ImageData
                Console.WriteLine($"Current ImageData: {(fillHelper.ImageData == null ? "null" : $"Length: {fillHelper.ImageData.Length} bytes")}");

                // Establece nuevos datos de imagen (crea una imagen roja simple de 1x1 píxel)
                byte[] imageData = new byte[] { 0x42, 0x4D, 0x3A, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x36, 0x00, 0x00, 0x00, 0x28, 0x00,
                                               0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x01, 0x00, 0x18, 0x00, 0x00, 0x00,
                                               0x00, 0x00, 0x04, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
                                               0x00, 0x00, 0x00, 0x00, 0x00, 0xFF, 0x00, 0x00 };

                fillHelper.ImageData = imageData;
                Console.WriteLine($"Updated ImageData length: {fillHelper.ImageData.Length} bytes");

                // Demuestra la lectura del valor de ImageData
                byte[] currentImageData = fillHelper.ImageData;
                Console.WriteLine($"Current ImageData length: {currentImageData.Length} bytes");

                // Guarda el libro de trabajo para demostrar una ejecución exitosa
                workbook.Save("ImageDataDemo.xlsx");

                Console.WriteLine("ImageData property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during ImageData demo: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


