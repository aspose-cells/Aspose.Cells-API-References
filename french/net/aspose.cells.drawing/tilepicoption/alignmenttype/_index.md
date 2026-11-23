---
title: "TilePicOption.AlignmentType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TilePicOption. Obtient ou définit l'alignement pour le carrelage"
type: docs
url: /fr/net/aspose.cells.drawing/tilepicoption/alignmenttype/
---
## TilePicOption.AlignmentType property

Obtient ou définit l'alignement du carrelage.

```csharp
public RectangleAlignmentType AlignmentType { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class TilePicOptionPropertyAlignmentTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme rectangulaire pour démontrer le carrelage
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 300, 300);

            // Configurez le format de remplissage pour utiliser une image en mosaïque
            FillFormat fillFormat = rectangle.Fill;
            fillFormat.FillType = FillType.Texture;

            // Créer et configurer TilePicOption
            TilePicOption tileOptions = new TilePicOption();
            
            // Afficher la valeur initiale de AlignmentType
            Console.WriteLine("Current AlignmentType: " + tileOptions.AlignmentType);

            // Définir l'alignement sur TopRight
            tileOptions.AlignmentType = RectangleAlignmentType.TopRight;
            tileOptions.ScaleX = 0.5;
            tileOptions.ScaleY = 0.5;

            // Appliquez les options de mosaïque au remplissage de la forme
            fillFormat.TextureFill.TilePicOption = tileOptions;

            // Charger l'image d'exemple (point rouge de 1x1 pixel)
            byte[] imageData = Convert.FromBase64String(
                "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVR42mNkYPhfDwAChwGA60e6kgAAAABJRU5ErkJggg==");
            fillFormat.ImageData = imageData;

            // Enregistrer le classeur modifié
            workbook.Save("TilePicOptionPropertyAlignmentTypeDemo.xlsx");

            // Modifier l'alignement en BottomLeft et enregistrer une autre version
            tileOptions.AlignmentType = RectangleAlignmentType.BottomLeft;
            workbook.Save("TilePicOptionPropertyAlignmentTypeDemo_BottomLeft.xlsx");
        }
    }
}
```

### Voir aussi

* enum [RectangleAlignmentType](../../rectanglealignmenttype/)
* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


