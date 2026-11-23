---
title: "ReflectionEffect.Size"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ReflectionEffect property. Obtient et définit la position finale le long de la rampe du dégradé alpha de la valeur alpha finale en unité de pourcentage"
type: docs
url: /fr/net/aspose.cells.drawing/reflectioneffect/size/
---
## ReflectionEffect.Size property

Obtient et définit la position finale (le long de la rampe de dégradé alpha) de la valeur alpha finale,in unités de pourcentage

```csharp
public double Size { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ReflectionEffectPropertySizeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            // Définissez les propriétés de réflexion incluant la taille
            ReflectionEffect reflection = shape.Reflection;
            reflection.Type = ReflectionEffectType.HalfReflection4PtOffset;
            reflection.Transparency = 0.5;
            reflection.Size = 55.5;
            reflection.Blur = 0.5;
            reflection.Distance = 4;

            // Enregistrez le classeur
            workbook.Save("output.xlsx");

            // Vérifiez les propriétés de réflexion enregistrées
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            ReflectionEffect loadedReflection = loadedShape.Reflection;

            Console.WriteLine("Reflection Size: " + loadedReflection.Size);
        }
    }
}
```

### Voir aussi

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


