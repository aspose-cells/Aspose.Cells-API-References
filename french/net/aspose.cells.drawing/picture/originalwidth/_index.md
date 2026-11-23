---
title: "Picture.OriginalWidth"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Picture. Obtient la largeur originale de l'image"
type: docs
url: /fr/net/aspose.cells.drawing/picture/originalwidth/
---
## Picture.OriginalWidth property

Obtient la largeur originale de l'image.

```csharp
public int OriginalWidth { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyOriginalWidthDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une image à la feuille de calcul
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
            Aspose.Cells.Drawing.Picture pic = worksheet.Pictures[imgIndex];

            // Obtenir et afficher la largeur originale de l'image
            int originalWidth = pic.OriginalWidth;
            Console.WriteLine("Original width of the picture: " + originalWidth + " pixels");

            // Enregistrez le classeur
            workbook.Save("result.xlsx");
        }
    }
}
```

### Voir aussi

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


