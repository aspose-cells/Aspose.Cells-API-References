---
title: "PicFormatOption.Right"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PicFormatOption. Obtient ou définit le décalage droit pour étirer l'image"
type: docs
url: /fr/net/aspose.cells.drawing/picformatoption/right/
---
## PicFormatOption.Right property

Obtient ou définit le décalage droit pour l'étirement de l'image.

```csharp
public double Right { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PicFormatOptionPropertyRightDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur et accéder à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme rectangulaire avec des dimensions spécifiées
            Shape shape = worksheet.Shapes.AddRectangle(5, 2, 10, 10, 150, 300);

            // Configurer le remplissage d'image pour la forme
            shape.Fill.FillType = FillType.Texture;
            string imagePath = "sample.jpg"; // Replace with actual image path
            
            if (File.Exists(imagePath))
            {
                shape.Fill.ImageData = File.ReadAllBytes(imagePath);
            }
            else
            {
                Console.WriteLine("Image not found - using empty picture fill");
            }

            // Accéder aux options de format d'image via TextureFill
            PicFormatOption picFormat = shape.Fill.TextureFill.PicFormatOption;

            // Afficher et modifier la propriété Right
            Console.WriteLine("Initial Right offset: " + picFormat.Right);
            picFormat.Right = 25.5; // Set right offset to 25.5 units

            // Vérifier la nouvelle valeur et enregistrer les modifications
            Console.WriteLine("Updated Right offset: " + picFormat.Right);
            workbook.Save("RightPropertyDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


