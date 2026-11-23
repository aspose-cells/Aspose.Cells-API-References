---
title: "TilePicOption.MirrorType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TilePicOption. Obtient ou définit le type de miroir pour la mosaïque"
type: docs
url: /fr/net/aspose.cells.drawing/tilepicoption/mirrortype/
---
## TilePicOption.MirrorType property

Obtient ou définit le type de miroir pour le carrelage.

```csharp
public MirrorType MirrorType { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class TilePicOptionPropertyMirrorTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme rectangulaire avec tous les paramètres requis
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 500, 500, 500);

            // Charge des données d'image d'exemple (remplacez par le chemin réel de l'image)
            byte[] imageData = File.ReadAllBytes("sample.png");

            // Créez et configurez une instance de TilePicOption
            TilePicOption tileOptions = new TilePicOption();

            // Afficher la valeur initiale de MirrorType
            Console.WriteLine("Current MirrorType: " + tileOptions.MirrorType);

            // Configurez les options de mosaïquage
            tileOptions.ScaleX = 0.5;
            tileOptions.ScaleY = 0.5;
            tileOptions.MirrorType = MirrorType.Both;

            // Appliquer la configuration du carrelage en utilisant les propriétés correctes
            shape.Fill.FillType = FillType.Texture;
            shape.Fill.ImageData = imageData;
            shape.Fill.TextureFill.TilePicOption = tileOptions;

            // Enregistrer le classeur modifié
            workbook.Save("TilePicOptionMirrorTypeDemo.xlsx");

            Console.WriteLine("Updated MirrorType: " + tileOptions.MirrorType);
        }
    }
}
```

### Voir aussi

* enum [MirrorType](../../mirrortype/)
* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


