---
title: "Shape.RelativeToOriginalPictureSize"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Indique si la forme est relative à la taille d'origine de l'image"
type: docs
url: /fr/net/aspose.cells.drawing/shape/relativetooriginalpicturesize/
---
## Shape.RelativeToOriginalPictureSize property

Indique si la forme est relative à la taille originale de l'image.

```csharp
public bool RelativeToOriginalPictureSize { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyRelativeToOriginalPictureSizeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une image à la feuille de calcul
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[index];

            // Accéder aux propriétés de la forme - Picture est déjà une Shape, aucune conversion nécessaire
            Shape shape = picture;

            // Démontrer la propriété RelativeToOriginalPictureSize
            Console.WriteLine("Original RelativeToOriginalPictureSize: " + shape.RelativeToOriginalPictureSize);
            
            // Modifier la propriété
            shape.RelativeToOriginalPictureSize = !shape.RelativeToOriginalPictureSize;
            Console.WriteLine("Modified RelativeToOriginalPictureSize: " + shape.RelativeToOriginalPictureSize);
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


