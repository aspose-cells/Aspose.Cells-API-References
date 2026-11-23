---
title: "DrawObject.ImageBytes"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DrawObject. Indique les octets d'image du Chart Shape rendu lors du rendu"
type: docs
url: /fr/net/aspose.cells.rendering/drawobject/imagebytes/
---
## DrawObject.ImageBytes property

Indique les octets d’image du graphique ou de la forme rendus lors du rendu.

```csharp
public byte[] ImageBytes { get; }
```

### Exemples

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
        // Gestionnaire d'événement personnalisé pour capturer les octets d'image
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
            // Créer un nouveau classeur et accéder à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // PNG 1x1 pixel rouge encodé en Base64
            byte[] generatedImageBytes = Convert.FromBase64String("iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVR42mNkYPhfDwAChwGA60e6kgAAAABJRU5ErkJggg==");

            // Ajouter l'image générée à la feuille de calcul en utilisant un flux
            using (MemoryStream imageStream = new MemoryStream(generatedImageBytes))
            {
                worksheet.Pictures.Add(0, 0, imageStream);
            }

            // Configurer les options de rendu
            ImageOrPrintOptions renderOptions = new ImageOrPrintOptions();
            renderOptions.ImageType = ImageType.Png;

            // Créer une instance du gestionnaire et l'assigner aux options
            var imageHandler = new ImageBytesHandler();
            renderOptions.DrawObjectEventHandler = imageHandler;

            SheetRender sheetRenderer = new SheetRender(worksheet, renderOptions);
            
            // Rendre la feuille de calcul pour déclencher l'événement DrawObject en utilisant un flux factice
            using (MemoryStream dummyStream = new MemoryStream())
            {
                sheetRenderer.ToImage(0, dummyStream);
            }

            // Ajouter l'image capturée à la feuille de calcul si disponible
            byte[] capturedImageBytes = imageHandler.CapturedImageBytes;
            if (capturedImageBytes != null)
            {
                int newRowPosition = worksheet.Cells.MaxDataRow + 2;
                using (MemoryStream capturedStream = new MemoryStream(capturedImageBytes))
                {
                    worksheet.Pictures.Add(newRowPosition, 0, capturedStream);
                }
            }

            // Enregistrer le classeur modifié
            workbook.Save("ImageBytesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


