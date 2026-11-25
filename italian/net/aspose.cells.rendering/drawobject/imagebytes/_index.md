---
title: "DrawObject.ImageBytes"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DrawObject. Indica i byte dell'immagine della Forma del Grafico renderizzata durante il rendering"
type: docs
url: /it/net/aspose.cells.rendering/drawobject/imagebytes/
---
## DrawObject.ImageBytes property

Indica i byte dell'immagine del grafico o della forma renderizzati durante il rendering.

```csharp
public byte[] ImageBytes { get; }
```

### Esempi

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
        // Gestore di eventi personalizzato per catturare i byte dell'immagine
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
            // Crea una nuova cartella di lavoro e accedi al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // PNG a pixel rosso 1x1 codificato in Base64
            byte[] generatedImageBytes = Convert.FromBase64String("iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVR42mNkYPhfDwAChwGA60e6kgAAAABJRU5ErkJggg==");

            // Aggiungi l'immagine generata al foglio di lavoro usando uno stream
            using (MemoryStream imageStream = new MemoryStream(generatedImageBytes))
            {
                worksheet.Pictures.Add(0, 0, imageStream);
            }

            // Configura le opzioni di rendering
            ImageOrPrintOptions renderOptions = new ImageOrPrintOptions();
            renderOptions.ImageType = ImageType.Png;

            // Crea un'istanza del gestore e assegnala alle opzioni
            var imageHandler = new ImageBytesHandler();
            renderOptions.DrawObjectEventHandler = imageHandler;

            SheetRender sheetRenderer = new SheetRender(worksheet, renderOptions);
            
            // Esegui il rendering del foglio di lavoro per attivare l'evento DrawObject usando uno stream fittizio
            using (MemoryStream dummyStream = new MemoryStream())
            {
                sheetRenderer.ToImage(0, dummyStream);
            }

            // Aggiungi l'immagine catturata al foglio di lavoro se disponibile
            byte[] capturedImageBytes = imageHandler.CapturedImageBytes;
            if (capturedImageBytes != null)
            {
                int newRowPosition = worksheet.Cells.MaxDataRow + 2;
                using (MemoryStream capturedStream = new MemoryStream(capturedImageBytes))
                {
                    worksheet.Pictures.Add(newRowPosition, 0, capturedStream);
                }
            }

            // Salvare la cartella di lavoro modificata
            workbook.Save("ImageBytesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


