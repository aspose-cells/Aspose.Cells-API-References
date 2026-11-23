---
title: "Shape.Reflection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Représente un objet ReflectionEffect qui spécifie l'effet de réflexion pour l'élément de graphique ou la forme"
type: docs
url: /fr/net/aspose.cells.drawing/shape/reflection/
---
## Shape.Reflection property

Représente un objet [`ReflectionEffect`](../../reflectioneffect/) qui spécifie l'effet de réflexion pour l'élément de graphique ou la forme.

```csharp
public ReflectionEffect Reflection { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyReflectionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme rectangulaire
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // Définir les propriétés de réflexion
            ReflectionEffect reflection = shape.Reflection;
            reflection.Blur = 5;
            reflection.Distance = 10;
            reflection.Direction = 90;
            reflection.FadeDirection = 90;
            reflection.Size = 50;
            reflection.Transparency = 0.5;
            reflection.Type = ReflectionEffectType.None;

            // Enregistrez le classeur
            workbook.Save("ShapeReflectionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ReflectionEffect](../../reflectioneffect/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


