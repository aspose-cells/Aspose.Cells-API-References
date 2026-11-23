---
title: "TilePicOption.OffsetX"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TilePicOption. Obtient ou définit le décalage X pour l'image en mosaïque"
type: docs
url: /fr/net/aspose.cells.drawing/tilepicoption/offsetx/
---
## TilePicOption.OffsetX property

Obtient ou définit le décalage X de l'image en mosaïque.

```csharp
public double OffsetX { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TilePicOptionPropertyOffsetXDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme rectangulaire pour démontrer le carrelage
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 200, 200);

            // Configurez le format de remplissage pour utiliser une image en mosaïque
            FillFormat fillFormat = rectangle.Fill;
            fillFormat.FillType = FillType.Texture;

            // Créer et configurer TilePicOption
            TilePicOption tileOptions = new TilePicOption();
            
            // Lisez la valeur initiale de OffsetX
            Console.WriteLine("Current OffsetX value: " + tileOptions.OffsetX);

            // Définissez un nouveau décalage X pour le motif en mosaïque
            tileOptions.OffsetX = 15.5;

            // Appliquez les options de mosaïque au remplissage de la forme
            fillFormat.TextureFill.TilePicOption = tileOptions;

            // Chargez une image minimale de 1x1 pixel (point rouge)
            byte[] imageData = Convert.FromBase64String(
                "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVR42mNkYPhfDwAChwGA60e6kgAAAABJRU5ErkJggg==");
            fillFormat.ImageData = imageData;

            // Enregistrer le classeur modifié
            workbook.Save("TilePicOptionPropertyOffsetXDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


