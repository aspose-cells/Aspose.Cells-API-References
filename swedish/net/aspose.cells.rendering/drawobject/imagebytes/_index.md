---
title: "DrawObject.ImageBytes"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DrawObject‑egenskap. Anger bildbytes för renderad Chart‑Shape vid rendering"
type: docs
url: /sv/net/aspose.cells.rendering/drawobject/imagebytes/
---
## DrawObject.ImageBytes property

Anger bildbytes för renderad Chart, Shape vid rendering.

```csharp
public byte[] ImageBytes { get; }
```

### Exempel

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
        // Anpassad händelsehanterare för att fånga bildbytes
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
            // Skapa en ny arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Base64‑kodad 1x1 röd pixel PNG
            byte[] generatedImageBytes = Convert.FromBase64String("iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVR42mNkYPhfDwAChwGA60e6kgAAAABJRU5ErkJggg==");

            // Lägg till den genererade bilden i kalkylbladet med en ström
            using (MemoryStream imageStream = new MemoryStream(generatedImageBytes))
            {
                worksheet.Pictures.Add(0, 0, imageStream);
            }

            // Ställ in renderingsalternativ
            ImageOrPrintOptions renderOptions = new ImageOrPrintOptions();
            renderOptions.ImageType = ImageType.Png;

            // Skapa en handler‑instans och tilldela den till alternativen
            var imageHandler = new ImageBytesHandler();
            renderOptions.DrawObjectEventHandler = imageHandler;

            SheetRender sheetRenderer = new SheetRender(worksheet, renderOptions);
            
            // Rendera kalkylbladet för att utlösa DrawObject‑händelsen med en dummy‑ström
            using (MemoryStream dummyStream = new MemoryStream())
            {
                sheetRenderer.ToImage(0, dummyStream);
            }

            // Lägg till den fångade bilden i kalkylbladet om den finns
            byte[] capturedImageBytes = imageHandler.CapturedImageBytes;
            if (capturedImageBytes != null)
            {
                int newRowPosition = worksheet.Cells.MaxDataRow + 2;
                using (MemoryStream capturedStream = new MemoryStream(capturedImageBytes))
                {
                    worksheet.Pictures.Add(newRowPosition, 0, capturedStream);
                }
            }

            // Spara modifierad arbetsbok
            workbook.Save("ImageBytesDemo.xlsx");
        }
    }
}
```

### Se även

* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


