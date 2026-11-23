---
title: "PicFormatOption.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PicFormatOption. Obtient ou définit le type de remplissage de l'image"
type: docs
url: /fr/net/aspose.cells.drawing/picformatoption/type/
---
## PicFormatOption.Type property

Obtient ou définit le type de remplissage de l'image.

```csharp
public FillPictureType Type { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PicFormatOptionPropertyTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une image BMP simple de 1x1 pixel
            byte[] bmpBytes = new byte[]
            {
                0x42, 0x4D, 0x39, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x36, 0x00, 0x00, 0x00,
                0x28, 0x00, 0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x01, 0x00,
                0x18, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
                0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
                0x00, 0x00, 0x00
            };

            // Ajouter une image à la feuille de calcul
            int pictureIndex = worksheet.Pictures.Add(0, 0, new MemoryStream(bmpBytes));
            Picture picture = worksheet.Pictures[pictureIndex];

            // Définir la position et la taille de l'image
            picture.UpperLeftRow = 0;
            picture.UpperLeftColumn = 0;
            picture.LowerRightRow = 5;
            picture.LowerRightColumn = 5;

            try
            {
                // Obtenir le PicFormatOption à partir du remplissage de texture de l'image
                PicFormatOption picFormat = picture.Fill.TextureFill.PicFormatOption;

                // Afficher la valeur actuelle de Type
                Console.WriteLine("Current Type: " + picFormat.Type);

                // Définir différentes valeurs de Type et les afficher
                picFormat.Type = FillPictureType.Stretch;
                Console.WriteLine("Type set to Stretch: " + picFormat.Type);

                picFormat.Type = FillPictureType.Stack;
                Console.WriteLine("Type set to Stack: " + picFormat.Type);

                picFormat.Type = FillPictureType.StackAndScale;
                Console.WriteLine("Type set to StackAndScale: " + picFormat.Type);

                // Enregistrez le classeur
                workbook.Save("PicFormatOptionTypeDemo.xlsx");
                Console.WriteLine("Type property demonstration completed successfully.");
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

* enum [FillPictureType](../../fillpicturetype/)
* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


