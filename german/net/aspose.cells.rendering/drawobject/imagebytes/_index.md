---
title: "DrawObject.ImageBytes"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DrawObject‑Eigenschaft. Gibt die Bildbytes des gerenderten Diagramm‑Shapes beim Rendern an"
type: docs
url: /de/net/aspose.cells.rendering/drawobject/imagebytes/
---
## DrawObject.ImageBytes property

Gibt die Bildbytes des gerenderten Diagramms, der Form beim Rendern an.

```csharp
public byte[] ImageBytes { get; }
```

### Beispiele

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
        // Benutzerdefinierter Ereignis‑Handler zum Erfassen von Bildbytes
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
            // Erstelle eine neue Arbeitsmappe und greife auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Base64‑kodiertes 1×1 rotes Pixel‑PNG
            byte[] generatedImageBytes = Convert.FromBase64String("iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVR42mNkYPhfDwAChwGA60e6kgAAAABJRU5ErkJggg==");

            // Fügen Sie das erzeugte Bild dem Arbeitsblatt mithilfe eines Streams hinzu
            using (MemoryStream imageStream = new MemoryStream(generatedImageBytes))
            {
                worksheet.Pictures.Add(0, 0, imageStream);
            }

            // Richten Sie Rendering‑Optionen ein
            ImageOrPrintOptions renderOptions = new ImageOrPrintOptions();
            renderOptions.ImageType = ImageType.Png;

            // Handler-Instanz erstellen und den Optionen zuweisen
            var imageHandler = new ImageBytesHandler();
            renderOptions.DrawObjectEventHandler = imageHandler;

            SheetRender sheetRenderer = new SheetRender(worksheet, renderOptions);
            
            // Arbeitsblatt rendern, um das DrawObject-Ereignis mit einem Dummy-Stream auszulösen
            using (MemoryStream dummyStream = new MemoryStream())
            {
                sheetRenderer.ToImage(0, dummyStream);
            }

            // Erfasstes Bild zum Arbeitsblatt hinzufügen, falls verfügbar
            byte[] capturedImageBytes = imageHandler.CapturedImageBytes;
            if (capturedImageBytes != null)
            {
                int newRowPosition = worksheet.Cells.MaxDataRow + 2;
                using (MemoryStream capturedStream = new MemoryStream(capturedImageBytes))
                {
                    worksheet.Pictures.Add(newRowPosition, 0, capturedStream);
                }
            }

            // Modifizierte Arbeitsmappe speichern
            workbook.Save("ImageBytesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


