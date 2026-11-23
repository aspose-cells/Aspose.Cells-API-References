---
title: "MsoFillFormat.Texture"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MsoFillFormat. Obtient le type de remplissage de texture"
type: docs
url: /fr/net/aspose.cells.drawing/msofillformat/texture/
---
## MsoFillFormat.Texture property

Obtient le type de remplissage de texture.

```csharp
public TextureType Texture { get; }
```

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme rectangulaire pour démontrer le formatage du remplissage
            var rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 150, 200);

            // Obtenir le format de remplissage
            MsoFillFormat fillFormat = rectangle.FillFormat;

            try
            {
                // Affichez le type de texture actuel (propriété en lecture seule)
                TextureType currentTexture = fillFormat.Texture;
                Console.WriteLine("Current Texture Type: " + currentTexture);

                // Définissez des données d'image pour éventuellement modifier la texture
                // Cela montre comment la texture peut être affectée par les données d'image
                byte[] sampleImageData = new byte[] { 0x89, 0x50, 0x4E, 0x47 }; // PNG header
                fillFormat.ImageData = sampleImageData;

                // Affichez à nouveau le type de texture après avoir défini les données d'image
                TextureType updatedTexture = fillFormat.Texture;
                Console.WriteLine("Texture Type after setting image data: " + updatedTexture);

                // Enregistrez le classeur
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

### Voir aussi

* enum [TextureType](../../texturetype/)
* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


