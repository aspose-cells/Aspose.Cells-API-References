---
title: "Shape.IsLockAspectRatio"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. True signifie que le ratio d'aspect de la forme est verrouillé"
type: docs
url: /fr/net/aspose.cells.drawing/shape/islockaspectratio/
---
## Shape.IsLockAspectRatio property

Vrai signifie que le rapport d'aspect de la forme est verrouillé.

```csharp
[Obsolete("Use Shape.IsAspectRatioLocked property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsLockAspectRatio { get; set; }
```

### Remarques

Uniquement pour les images et les objets Ole. NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété Shape.IsAspectRatioLocked. Cette propriété sera supprimée 12 mois plus tard à compter de juillet 2024. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsLockAspectRatioDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme rectangulaire avec tous les paramètres requis
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Verrouiller le ratio d'aspect
            shape.IsLockAspectRatio = true;
            Console.WriteLine("Aspect ratio locked: " + shape.IsLockAspectRatio);

            // Déverrouiller le ratio d'aspect
            shape.IsLockAspectRatio = false;
            Console.WriteLine("Aspect ratio locked: " + shape.IsLockAspectRatio);
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


