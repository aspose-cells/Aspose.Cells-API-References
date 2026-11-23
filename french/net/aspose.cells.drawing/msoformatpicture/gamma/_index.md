---
title: "MsoFormatPicture.Gamma"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MsoFormatPicture. Représente le gamma de l'image"
type: docs
url: /fr/net/aspose.cells.drawing/msoformatpicture/gamma/
---
## MsoFormatPicture.Gamma property

Représente le gamma de l'image.

```csharp
public double Gamma { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyGammaDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter une image à la feuille de calcul (en utilisant un chemin d'image d'exemple)
            int pictureIndex = sheet.Pictures.Add(5, 5, "sample.jpg");
            Picture picture = sheet.Pictures[pictureIndex];

            // Accédez à l'objet MsoFormatPicture
            MsoFormatPicture formatPicture = picture.FormatPicture;

            // Définir la propriété Gamma
            formatPicture.Gamma = 1.5; // Demonstrating Gamma adjustment

            // Enregistrez le classeur
            workbook.Save("MsoFormatPictureGammaDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


