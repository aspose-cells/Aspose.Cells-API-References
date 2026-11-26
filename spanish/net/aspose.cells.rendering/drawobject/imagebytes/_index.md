---
title: "DrawObject.ImageBytes"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DrawObject. Indica los bytes de imagen de la Chart Shape renderizada al renderizar"
type: docs
url: /es/net/aspose.cells.rendering/drawobject/imagebytes/
---
## DrawObject.ImageBytes property

Indica los bytes de imagen del Chart o Shape renderizado al renderizar.

```csharp
public byte[] ImageBytes { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class DrawObjectPropertyImageBytesDemo
    {
        // Manejador de eventos personalizado para capturar los bytes de imagen
        private class ImageBytesHandler : DrawObjectEventHandler
        {
            public byte[] CapturedImageBytes { get; private set; }

            public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
            {
                if (drawObject.Type == DrawObjectEnum.Image)
                {
                    CapturedImageBytes = drawObject.ImageBytes;
                    Console.WriteLine($"Captured image size: {CapturedImageBytes?.Length ?? 0} bytes");
                }
            }
        }

        public static void Run()
        {
            // Crear un nuevo libro de trabajo y acceder a la primera hoja
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // PNG de píxel rojo 1x1 codificado en Base64
            byte[] generatedImageBytes = Convert.FromBase64String("iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVR42mNkYPhfDwAChwGA60e6kgAAAABJRU5ErkJggg==");

            // Añade la imagen generada a la hoja de cálculo usando un flujo
            using (MemoryStream imageStream = new MemoryStream(generatedImageBytes))
            {
                worksheet.Pictures.Add(0, 0, imageStream);
            }

            // Configura las opciones de renderizado
            ImageOrPrintOptions renderOptions = new ImageOrPrintOptions();
            renderOptions.ImageType = ImageType.Png;

            // Crea una instancia del manejador y asígnala a las opciones
            var imageHandler = new ImageBytesHandler();
            renderOptions.DrawObjectEventHandler = imageHandler;

            SheetRender sheetRenderer = new SheetRender(worksheet, renderOptions);
            
            // Renderiza la hoja de cálculo para activar el evento DrawObject usando un flujo ficticio
            using (MemoryStream dummyStream = new MemoryStream())
            {
                sheetRenderer.ToImage(0, dummyStream);
            }

            // Añade la imagen capturada a la hoja de cálculo si está disponible
            byte[] capturedImageBytes = imageHandler.CapturedImageBytes;
            if (capturedImageBytes != null)
            {
                int newRowPosition = worksheet.Cells.MaxDataRow + 2;
                using (MemoryStream capturedStream = new MemoryStream(capturedImageBytes))
                {
                    worksheet.Pictures.Add(newRowPosition, 0, capturedStream);
                }
            }

            // Guardar el libro de trabajo modificado
            workbook.Save("ImageBytesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


