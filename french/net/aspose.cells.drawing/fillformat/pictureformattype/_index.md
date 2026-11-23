---
title: "FillFormat.PictureFormatType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FillFormat. Obtient et définit le type de format d'image"
type: docs
url: /fr/net/aspose.cells.drawing/fillformat/pictureformattype/
---
## FillFormat.PictureFormatType property

Obtient et définit le type de format d'image.

```csharp
public FillPictureType PictureFormatType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyPictureFormatTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme pour démontrer le remplissage d'image
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 200);

            // Définir les propriétés du remplissage d'image
            shape.Fill.Type = FillType.Texture;
            shape.Fill.Texture = TextureType.BlueTissuePaper;
            shape.Fill.PictureFormatType = FillPictureType.Stretch;

            // Enregistrez le classeur
            workbook.Save("FillFormatPictureTypeDemo.xlsx");

            // Chargez le classeur enregistré pour vérifier les propriétés
            Workbook verifyWorkbook = new Workbook("FillFormatPictureTypeDemo.xlsx");
            Shape verifyShape = verifyWorkbook.Worksheets[0].Shapes[0];

            // Affichez le PictureFormatType pour démontrer son utilisation
            Console.WriteLine("PictureFormatType: " + verifyShape.Fill.PictureFormatType);
        }
    }
}
```

### Voir aussi

* enum [FillPictureType](../../fillpicturetype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


