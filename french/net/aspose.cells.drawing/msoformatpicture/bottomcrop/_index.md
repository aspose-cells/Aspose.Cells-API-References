---
title: "MsoFormatPicture.BottomCrop"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MsoFormatPicture. Représente l'emplacement du bas du rectangle de recadrage exprimé comme un ratio de la hauteur de l'image"
type: docs
url: /fr/net/aspose.cells.drawing/msoformatpicture/bottomcrop/
---
## MsoFormatPicture.BottomCrop property

Représente l'emplacement du bas du rectangle de recadrage exprimé comme un ratio de la hauteur de l'image.

```csharp
public double BottomCrop { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoFormatPicturePropertyBottomCropDemo
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

            // Afficher la valeur actuelle de BottomCrop
            Console.WriteLine("Current BottomCrop value: " + msoFormatPicture.BottomCrop);

            // Définir une nouvelle valeur BottomCrop (0,2 signifie recadrer 20 % depuis le bas)
            msoFormatPicture.BottomCrop = 0.2;
            Console.WriteLine("BottomCrop set to: " + msoFormatPicture.BottomCrop);

            // Définir d'autres valeurs de recadrage pour démontrer l'effet
            msoFormatPicture.TopCrop = 0.1;
            msoFormatPicture.LeftCrop = 0.1;
            msoFormatPicture.RightCrop = 0.1;

            // Enregistrer le classeur pour voir l'image recadrée
            workbook.Save("MsoFormatPicturePropertyBottomCropDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


