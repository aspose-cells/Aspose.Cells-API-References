---
title: "MsoFormatPicture.LeftCrop"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MsoFormatPicture. Représente la position du côté gauche du rectangle de recadrage exprimée comme un ratio de la largeur de l'image"
type: docs
url: /fr/net/aspose.cells.drawing/msoformatpicture/leftcrop/
---
## MsoFormatPicture.LeftCrop property

Représente l'emplacement du côté gauche du rectangle de recadrage exprimé comme un ratio de la largeur de l'image.

```csharp
public double LeftCrop { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyLeftCropDemo
    {
        public static void Run()
        {
            // Créer un classeur
            var workbook = new Workbook();
            var sheet = workbook.Worksheets[0];

            // Charger les données d'image
            byte[] imageData = File.ReadAllBytes("example.png");
            
            // Ajouter une image à la feuille de calcul
            int pictureIndex = sheet.Pictures.Add(0, 0, new MemoryStream(imageData));
            var picture = sheet.Pictures[pictureIndex];

            // Définir la propriété LeftCrop
            picture.FormatPicture.LeftCrop = 0.1;
            Console.WriteLine("LeftCrop set to: " + picture.FormatPicture.LeftCrop);

            // Obtenir et définir la propriété LeftCropInch
            double leftCropInch = picture.FormatPicture.LeftCropInch;
            picture.FormatPicture.LeftCropInch = leftCropInch;
            Console.WriteLine("LeftCropInch value: " + leftCropInch);

            // Enregistrez le classeur
            workbook.Save("LeftCropDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


