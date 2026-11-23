---
title: "Enum MirrorType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.MirrorType enum. Représente le type de miroir du remplissage de texture"
type: docs
url: /fr/net/aspose.cells.drawing/mirrortype/
---
## MirrorType enumeration

Représente le type de miroir du remplissage de texture

```csharp
public enum MirrorType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Aucun |
| Horizonal | `1` | Horizontal |
| Vertical | `2` | Vertical |
| Both | `3` | Les deux |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassMirrorTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme pour démontrer MirrorType
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 200);

            // Définir le remplissage de texture avec différents types de miroir
            shape.Fill.TextureFill.TilePicOption.MirrorType = MirrorType.Horizonal;
            shape = worksheet.Shapes.AddRectangle(2, 0, 1, 100, 100, 200);
            shape.Fill.TextureFill.TilePicOption.MirrorType = MirrorType.Vertical;
            shape = worksheet.Shapes.AddRectangle(3, 0, 1, 100, 100, 200);
            shape.Fill.TextureFill.TilePicOption.MirrorType = MirrorType.Both;
            shape = worksheet.Shapes.AddRectangle(4, 0, 1, 100, 100, 200);
            shape.Fill.TextureFill.TilePicOption.MirrorType = MirrorType.None;

            // Enregistrer le résultat
            workbook.Save("MirrorTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


