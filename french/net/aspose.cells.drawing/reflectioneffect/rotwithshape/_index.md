---
title: "ReflectionEffect.RotWithShape"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ReflectionEffect property. Obtient et définit si la réflexion doit pivoter avec la forme"
type: docs
url: /fr/net/aspose.cells.drawing/reflectioneffect/rotwithshape/
---
## ReflectionEffect.RotWithShape property

Obtient et définit si la réflexion doit pivoter avec la forme.

```csharp
public bool RotWithShape { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ReflectionEffectPropertyRotWithShapeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme à la feuille de calcul
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // Créez et appliquez l'effet de réflexion
            ReflectionEffect reflection = shape.Reflection;
            reflection.Type = ReflectionEffectType.FullReflection4PtOffset;
            reflection.Blur = 5;
            reflection.Distance = 10;
            reflection.Transparency = 0.3;

            // Affichez la valeur actuelle de RotWithShape
            Console.WriteLine("Current RotWithShape value: " + reflection.RotWithShape);

            // Définissez RotWithShape sur true
            reflection.RotWithShape = true;
            Console.WriteLine("RotWithShape set to: " + reflection.RotWithShape);

            // Faites pivoter la forme pour démontrer l'effet
            shape.RotationAngle = 45;

            // Enregistrez le classeur
            workbook.Save("ReflectionEffectRotWithShapeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


