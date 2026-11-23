---
title: "MsoFormatPicture.LeftCropInch"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MsoFormatPicture. Représente la position du côté gauche du rectangle de recadrage exprimée en pouces"
type: docs
url: /fr/net/aspose.cells.drawing/msoformatpicture/leftcropinch/
---
## MsoFormatPicture.LeftCropInch property

Représente l'emplacement du côté gauche du rectangle de recadrage exprimé en pouces.

```csharp
public double LeftCropInch { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyLeftCropInchDemo
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

            // Définir et obtenir la propriété LeftCropInch
            picture.FormatPicture.LeftCropInch = 0.5;
            double leftCropValue = picture.FormatPicture.LeftCropInch;

            Console.WriteLine($"Left crop value in inches: {leftCropValue}");

            // Enregistrez le classeur
            workbook.Save("LeftCropInchDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


