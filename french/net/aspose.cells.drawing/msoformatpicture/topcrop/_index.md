---
title: "MsoFormatPicture.TopCrop"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MsoFormatPicture. Représente l'emplacement du haut du rectangle de recadrage exprimé comme un ratio de la hauteur de l'image"
type: docs
url: /fr/net/aspose.cells.drawing/msoformatpicture/topcrop/
---
## MsoFormatPicture.TopCrop property

Représente l'emplacement du haut du rectangle de recadrage exprimé comme un ratio de la hauteur de l'image.

```csharp
public double TopCrop { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyTopCropDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une image à la feuille de calcul
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[index];
            
            // Définir la propriété TopCrop
            picture.FormatPicture.TopCrop = -6;
            
            // Afficher la valeur TopCrop
            Console.WriteLine("Picture TopCrop value: " + picture.FormatPicture.TopCrop);
            
            // Enregistrez le classeur
            workbook.Save("TopCropDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


