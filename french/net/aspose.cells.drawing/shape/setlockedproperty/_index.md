---
title: "Shape.SetLockedProperty"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Shape. Définir la propriété verrouillée"
type: docs
url: /fr/net/aspose.cells.drawing/shape/setlockedproperty/
---
## Shape.SetLockedProperty method

Définir la propriété locked.

```csharp
public void SetLockedProperty(ShapeLockType type, bool value)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | ShapeLockType | Le type verrouillé. |
| valeur | Boolean | La valeur de la propriété. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodSetLockedPropertyWithShapeLockTypeBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme d'exemple avec tous les paramètres requis
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 50);

            // Démontrez l'utilisation de SetLockedProperty
            shape.SetLockedProperty(ShapeLockType.AdjustHandles, true);
            shape.SetLockedProperty(ShapeLockType.Selection, false);

            Console.WriteLine("Shape locked properties set successfully.");
        }
    }
}
```

### Voir aussi

* enum [ShapeLockType](../../shapelocktype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


