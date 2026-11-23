---
title: "Enum LightRigDirectionType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.LightRigDirectionType enum. Représente le type de direction du dispositif d’éclairage"
type: docs
url: /fr/net/aspose.cells.drawing/lightrigdirectiontype/
---
## LightRigDirectionType enumeration

Représente le type de direction du dispositif d’éclairage.

```csharp
public enum LightRigDirectionType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Bottom | `0` | Bas |
| BottomLeft | `1` | En bas à gauche. |
| BottomRight | `2` | En bas à droite. |
| Left | `3` | Gauche. |
| Right | `4` | Droite. |
| Top | `5` | Haut. |
| TopLeft | `6` | En haut à gauche. |
| TopRight | `7` | Haut à droite. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassLightRigDirectionTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme pour démontrer la direction du dispositif d'éclairage
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 10, 10, 200, 200, 0, 0);

            // Définissez la direction du dispositif d'éclairage pour le format 3D de la forme
            shape.ThreeDFormat.LightingDirection = LightRigDirectionType.TopRight;

            // Démontrez différentes directions du dispositif d'éclairage
            Console.WriteLine("Current Light Rig Direction: " + shape.ThreeDFormat.LightingDirection);

            // Modifiez la direction du dispositif d'éclairage
            shape.ThreeDFormat.LightingDirection = LightRigDirectionType.BottomLeft;
            Console.WriteLine("Changed Light Rig Direction: " + shape.ThreeDFormat.LightingDirection);

            // Parcourez toutes les directions possibles du dispositif d'éclairage
            Console.WriteLine("\nAll Light Rig Direction Types:");
            foreach (LightRigDirectionType direction in Enum.GetValues(typeof(LightRigDirectionType)))
            {
                Console.WriteLine(direction.ToString());
            }

            // Enregistrez le classeur
            workbook.Save("LightRigDirectionTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


