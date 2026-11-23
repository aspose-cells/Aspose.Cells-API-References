---
title: "Énumération ShapeLockType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.Drawing.ShapeLockType. Représente le type de la propriété à verrouiller"
type: docs
url: /fr/net/aspose.cells.drawing/shapelocktype/
---
## ShapeLockType enumeration

Représente le type de la propriété à verrouiller.

```csharp
public enum ShapeLockType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Group | `0` | Groupe |
| AdjustHandles | `1` | AdjustHandles |
| Text | `2` | Texte |
| Points | `3` | Points |
| Crop | `4` | Crop |
| Selection | `5` | Selection |
| Move | `6` | Move |
| AspectRatio | `7` | AspectRatio |
| Rotation | `8` | Rotation |
| Ungroup | `9` | Ungroup |
| Resize | `10` | Resize |
| ShapeType | `11` | ShapeType |
| Arrowhead | `12` | Arrowhead |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassShapeLockTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une image à la feuille de calcul
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[index];

            // Démontrer la fonctionnalité de ShapeLockType
            picture.SetLockedProperty(Aspose.Cells.Drawing.ShapeLockType.AspectRatio, false);
            bool isAspectRatioLocked = picture.GetLockedProperty(Aspose.Cells.Drawing.ShapeLockType.AspectRatio);

            Console.WriteLine("Aspect Ratio locked: " + isAspectRatioLocked);

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


