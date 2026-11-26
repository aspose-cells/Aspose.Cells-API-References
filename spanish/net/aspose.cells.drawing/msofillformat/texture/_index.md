---
title: "MsoFillFormat.Texture"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MsoFillFormat. Obtiene el tipo de relleno de textura"
type: docs
url: /es/net/aspose.cells.drawing/msofillformat/texture/
---
## MsoFillFormat.Texture property

Obtiene el tipo de relleno de textura.

```csharp
public TextureType Texture { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoFillFormatPropertyTextureDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega una forma rectangular para demostrar el formato de relleno
            var rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 150, 200);

            // Obtener el formato de relleno
            MsoFillFormat fillFormat = rectangle.FillFormat;

            try
            {
                // Muestra el tipo de textura actual (propiedad de solo lectura)
                TextureType currentTexture = fillFormat.Texture;
                Console.WriteLine("Current Texture Type: " + currentTexture);

                // Establece algunos datos de imagen para cambiar potencialmente la textura
                // Esto demuestra cómo la textura puede verse afectada por los datos de imagen
                byte[] sampleImageData = new byte[] { 0x89, 0x50, 0x4E, 0x47 }; // PNG header
                fillFormat.ImageData = sampleImageData;

                // Muestra el tipo de textura nuevamente después de establecer los datos de imagen
                TextureType updatedTexture = fillFormat.Texture;
                Console.WriteLine("Texture Type after setting image data: " + updatedTexture);

                // Guarda el libro de trabajo
                workbook.Save("TextureDemo.xlsx");
                Console.WriteLine("Texture demonstration completed successfully.");
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

* enum [TextureType](../../texturetype/)
* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


