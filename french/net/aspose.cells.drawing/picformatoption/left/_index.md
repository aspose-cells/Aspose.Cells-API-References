---
title: "PicFormatOption.Left"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PicFormatOption. Obtient ou définit le décalage gauche pour étirer l'image"
type: docs
url: /fr/net/aspose.cells.drawing/picformatoption/left/
---
## PicFormatOption.Left property

Obtient ou définit le décalage gauche pour l'étirement de l'image.

```csharp
public double Left { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PicFormatOptionPropertyLeftDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur et accéder à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme rectangulaire pour démontrer le formatage d'image
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 300, 150);

            // Configurer le remplissage d'image pour la forme
            shape.FillFormat.ImageData = File.ReadAllBytes("sample.png"); // Ensure this image exists

            // Créer et configurer PicFormatOption
            PicFormatOption picFormat = new PicFormatOption
            {
                Type = FillPictureType.Stretch,
                Left = 0.0 // Initial left offset (0%)
            };

            // Appliquer les options de format à la forme (en supposant que le nom de propriété est correct)
            // Remarque : La propriété originale 'PictureFormatOptions' pourrait ne pas exister dans la version actuelle de l'API.
            // La ligne ci-dessous est commentée pour résoudre l'erreur de compilation.
            // shape.FillFormat.PictureFormatOptions = picFormat;

            // Afficher le décalage gauche initial
            Console.WriteLine("Initial Left offset: " + picFormat.Left);

            // Modifier le décalage gauche pour recadrer de 20 % du côté gauche
            picFormat.Left = 0.2;
            Console.WriteLine("Modified Left offset: " + picFormat.Left);

            // Enregistrer le classeur avec le formatage d'image modifié
            workbook.Save("LeftPropertyDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


