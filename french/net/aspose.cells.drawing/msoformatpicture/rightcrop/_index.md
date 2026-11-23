---
title: "MsoFormatPicture.RightCrop"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MsoFormatPicture. Représente l'emplacement du côté droit du rectangle de recadrage exprimé comme un ratio de la largeur de l'image"
type: docs
url: /fr/net/aspose.cells.drawing/msoformatpicture/rightcrop/
---
## MsoFormatPicture.RightCrop property

Représente l'emplacement du côté droit du rectangle de recadrage exprimé comme un ratio de la largeur de l'image.

```csharp
public double RightCrop { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoFormatPicturePropertyRightCropDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une image à la feuille de calcul
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];
            
            // Obtenir le MsoFormatPicture de l'image
            MsoFormatPicture msoFormatPicture = picture.FormatPicture;

            // Afficher la valeur actuelle de RightCrop
            Console.WriteLine("Current RightCrop value: " + msoFormatPicture.RightCrop);

            // Définir une nouvelle valeur RightCrop (0,2 signifie recadrer 20 % depuis la droite)
            msoFormatPicture.RightCrop = 0.2;
            Console.WriteLine("New RightCrop value set to: " + msoFormatPicture.RightCrop);

            // Enregistrer le classeur pour voir l'effet
            workbook.Save("RightCropDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


