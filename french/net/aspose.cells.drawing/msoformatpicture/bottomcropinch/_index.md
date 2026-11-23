---
title: "MsoFormatPicture.BottomCropInch"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MsoFormatPicture. Représente l'emplacement du bas du rectangle de recadrage exprimé en pouces"
type: docs
url: /fr/net/aspose.cells.drawing/msoformatpicture/bottomcropinch/
---
## MsoFormatPicture.BottomCropInch property

Représente l'emplacement du bas du rectangle de recadrage exprimé en pouces.

```csharp
public double BottomCropInch { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyBottomCropInchDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter une image à la feuille de calcul (en utilisant un chemin factice)
            int pictureIndex = sheet.Pictures.Add(5, 5, "sample.jpg");
            Picture picture = sheet.Pictures[pictureIndex];

            // Accédez à l'objet MsoFormatPicture
            MsoFormatPicture formatPicture = picture.FormatPicture;

            // Définir la propriété BottomCropInch et démontrer son utilisation
            formatPicture.BottomCropInch = 0.3;
            formatPicture.TopCropInch = 0.2;
            
            // Enregistrez le classeur
            workbook.Save("MsoFormatPictureBottomCropDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


