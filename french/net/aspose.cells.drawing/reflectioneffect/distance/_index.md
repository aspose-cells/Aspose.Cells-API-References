---
title: "ReflectionEffect.Distance"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ReflectionEffect property. Obtient et définit la distance de l'ombre en unité de points"
type: docs
url: /fr/net/aspose.cells.drawing/reflectioneffect/distance/
---
## ReflectionEffect.Distance property

Obtient et définit la distance de l'ombre,in unités de points.

```csharp
public double Distance { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ReflectionEffectPropertyDistanceDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme pour tester la réflexion - paramètres fixes pour correspondre à la signature de la méthode
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Définir les propriétés de réflexion
            ReflectionEffect reflection = shape.Reflection;
            reflection.Type = ReflectionEffectType.HalfReflection4PtOffset;
            reflection.Transparency = 0.5;
            reflection.Size = 55.5;
            reflection.Blur = 0.5;
            reflection.Distance = 4; // Demonstrating Distance property

            // Enregistrer et recharger pour vérifier la persistance
            string outputPath = "ReflectionEffectDemo.xlsx";
            workbook.Save(outputPath);

            // Recharger pour vérifier
            Workbook loadedWorkbook = new Workbook(outputPath);
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            ReflectionEffect loadedReflection = loadedShape.Reflection;

            Console.WriteLine("Original Distance: " + reflection.Distance);
            Console.WriteLine("Loaded Distance: " + loadedReflection.Distance);
        }
    }
}
```

### Voir aussi

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


