---
title: "FillFormat.ImageData"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FillFormat. Obtient et définit les données d'image"
type: docs
url: /fr/net/aspose.cells.drawing/fillformat/imagedata/
---
## FillFormat.ImageData property

Obtient et définit les données d'image.

```csharp
public byte[] ImageData { get; set; }
```

### Remarques

Si le format de remplissage n'est pas un format de texture personnalisé, retourne null.

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyImageDataDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une image d'exemple à la feuille de calcul
            string imagePath = "example.png";
            worksheet.Pictures.Add(0, 0, imagePath);

            // Créer un commentaire et définir les données d'image
            var comment = worksheet.Comments[worksheet.Comments.Add(2, 5)];
            byte[] imageData = File.ReadAllBytes(imagePath);
            comment.CommentShape.Fill.ImageData = imageData;

            // Enregistrer le classeur
            workbook.Save("FillFormatPropertyImageDataDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


