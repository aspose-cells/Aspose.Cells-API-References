---
title: "Énumération PresetShadowType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.Drawing.PresetShadowType. Représente le type d'ombre prédéfini"
type: docs
url: /fr/net/aspose.cells.drawing/presetshadowtype/
---
## PresetShadowType enumeration

Représente le type d’ombre prédéfini.

```csharp
public enum PresetShadowType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| NoShadow | `0` | Pas d'ombre. |
| Custom | `1` | Ombre personnalisée. |
| OffsetDiagonalBottomRight | `2` | Décalage d'ombre extérieure en diagonale en bas à droite. |
| OffsetBottom | `3` | Décalage d'ombre extérieure en bas. |
| OffsetDiagonalBottomLeft | `4` | Décalage de l'ombre externe en diagonale en bas à gauche. |
| OffsetRight | `5` | Décalage de l'ombre externe à droite. |
| OffsetCenter | `6` | Décalage de l'ombre externe au centre. |
| OffsetLeft | `7` | Décalage de l'ombre externe à gauche. |
| OffsetDiagonalTopRight | `8` | Décalage de l'ombre externe en diagonale en haut à droite. |
| OffsetTop | `9` | Décalage de l'ombre externe en haut. |
| OffsetDiagonalTopLeft | `10` | Décalage de l'ombre externe en diagonale en haut à gauche. |
| InsideDiagonalTopLeft | `11` | Ombre interne à l'intérieur en diagonale en haut à gauche. |
| InsideTop | `12` | Ombre interne à l'intérieur en haut. |
| InsideDiagonalTopRight | `13` | Ombre interne à l'intérieur en diagonale en haut à droite. |
| InsideLeft | `14` | Ombre interne à l'intérieur à gauche. |
| InsideCenter | `15` | Ombre interne à l'intérieur au centre. |
| InsideRight | `16` | Ombre interne à l'intérieur à droite. |
| InsideDiagonalBottomLeft | `17` | Ombre interne à l'intérieur en diagonale en bas à gauche. |
| InsideBottom | `18` | Ombre interne à l'intérieur en bas. |
| InsideDiagonalBottomRight | `19` | Ombre interne à l'intérieur en diagonale en bas à droite. |
| PerspectiveDiagonalUpperLeft | `20` | Perspective d'ombre externe en diagonale en haut à gauche. |
| PerspectiveDiagonalUpperRight | `21` | Perspective d'ombre externe en diagonale en haut à droite. |
| Below | `22` | Ombre externe en dessous. |
| PerspectiveDiagonalLowerLeft | `23` | Perspective d'ombre externe en diagonale en bas à gauche. |
| PerspectiveDiagonalLowerRight | `24` | Perspective d'ombre externe en diagonale en bas à droite. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassPresetShadowTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme pour démontrer les effets d'ombre
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            
            // Définissez différents types d'ombre prédéfinis
            shape.ShadowEffect.PresetType = PresetShadowType.OffsetDiagonalBottomRight;
            Console.WriteLine("Shadow type set to: " + shape.ShadowEffect.PresetType);

            // Changez pour un autre type d'ombre
            shape.ShadowEffect.PresetType = PresetShadowType.OffsetBottom;
            Console.WriteLine("Shadow type changed to: " + shape.ShadowEffect.PresetType);

            // Enregistrez le classeur
            workbook.Save("PresetShadowTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


