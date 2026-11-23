---
title: "Enum BevelType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.BevelType enum. Représente un préréglage pour un type de biseau qui peut être appliqué à une forme en 3D"
type: docs
url: /fr/net/aspose.cells.drawing/beveltype/
---
## BevelType enumeration

Représente un préréglage pour un type de biseau qui peut être appliqué à une forme en 3D.

```csharp
public enum BevelType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Pas de biseau |
| Angle | `1` | Angle |
| ArtDeco | `2` | Art déco |
| Circle | `3` | Cercle |
| Convex | `4` | Convexe |
| CoolSlant | `5` | Inclinaison cool |
| Cross | `6` | Croix |
| Divot | `7` | Creux |
| HardEdge | `8` | Bord dur |
| RelaxedInset | `9` | Encart détendu |
| Riblet | `10` | Riblet |
| Slope | `11` | Pente |
| SoftRound | `12` | Arrondi doux |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class BevelTypeDemo
    {
        public static void BevelTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme à la feuille de calcul
            var shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 0, 2, 0, 100, 100);

            // Accéder au format 3D de la forme
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Définir le type de chanfrein supérieur et ses dimensions
            threeDFormat.TopBevelType = BevelType.SoftRound;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;

            // Définir le type de chanfrein inférieur et ses dimensions
            threeDFormat.BottomBevelType = BevelType.Divot;
            threeDFormat.BottomBevelWidth = 5;
            threeDFormat.BottomBevelHeight = 5;

            // Enregistrez le classeur
            workbook.Save("BevelTypeExample.xlsx");
            workbook.Save("BevelTypeExample.pdf");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


