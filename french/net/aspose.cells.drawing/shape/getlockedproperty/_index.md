---
title: "Shape.GetLockedProperty"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Shape. Obtient la valeur de la propriété verrouillée"
type: docs
url: /fr/net/aspose.cells.drawing/shape/getlockedproperty/
---
## Shape.GetLockedProperty method

Obtient la valeur de la propriété locked.

```csharp
public bool GetLockedProperty(ShapeLockType type)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | ShapeLockType | Le type de la propriété verrouillée de la forme. |

### Valeur de retour

Renvoie la valeur de la propriété verrouillée.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetLockedPropertyWithShapeLockTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme à la feuille de calcul
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // Définir la propriété verrouillée pour AdjustHandles
            shape.SetLockedProperty(ShapeLockType.AdjustHandles, true);

            // Vérifier si AdjustHandles est verrouillé
            int noAdjustHandles = 0;
            if (shape.GetLockedProperty(ShapeLockType.AdjustHandles))
                noAdjustHandles = 1;

            Console.WriteLine("AdjustHandles locked status: " + (noAdjustHandles == 1));
        }
    }
}
```

### Voir aussi

* enum [ShapeLockType](../../shapelocktype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


