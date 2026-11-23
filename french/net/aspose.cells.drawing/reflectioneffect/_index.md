---
title: "Classe ReflectionEffect"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.ReflectionEffect. Cette classe spécifie un effet de réflexion"
type: docs
url: /fr/net/aspose.cells.drawing/reflectioneffect/
---
## ReflectionEffect class

Cette classe spécifie un effet de réflexion.

```csharp
public class ReflectionEffect
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Blur](../../aspose.cells.drawing/reflectioneffect/blur/) { get; set; } | Obtient et définit le rayon du flou,in unités de points. |
| [Direction](../../aspose.cells.drawing/reflectioneffect/direction/) { get; set; } | Obtient et définit la direction de la rampe de dégradé alpha par rapport à la forme elle-même. |
| [Distance](../../aspose.cells.drawing/reflectioneffect/distance/) { get; set; } | Obtient et définit la distance de l'ombre,in unités de points. |
| [FadeDirection](../../aspose.cells.drawing/reflectioneffect/fadedirection/) { get; set; } | Obtient et définit la direction du décalage de la réflexion. |
| [RotWithShape](../../aspose.cells.drawing/reflectioneffect/rotwithshape/) { get; set; } | Obtient et définit si la réflexion doit pivoter avec la forme. |
| [Size](../../aspose.cells.drawing/reflectioneffect/size/) { get; set; } | Obtient et définit la position finale (le long de la rampe de dégradé alpha) de la valeur alpha finale,in unités de pourcentage |
| [Transparency](../../aspose.cells.drawing/reflectioneffect/transparency/) { get; set; } | Obtient et définit le degré de transparence initiale de la réflexion comme une valeur de 0.0 (opaque) à 1.0 (clear). |
| [Type](../../aspose.cells.drawing/reflectioneffect/type/) { get; set; } | Obtient et définit l'effet de réflexion prédéfini. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassReflectionEffectDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme d'exemple
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // Définir les propriétés de l'effet de réflexion
            ReflectionEffect reflection = shape.Reflection;
            reflection.Size = 90;
            reflection.Blur = 30;
            reflection.Transparency = 0.5;
            reflection.Distance = 10;

            // Afficher les propriétés de réflexion
            Console.WriteLine("Reflection Size: " + reflection.Size);
            Console.WriteLine("Reflection Blur: " + reflection.Blur);
            Console.WriteLine("Reflection Transparency: " + reflection.Transparency);
            Console.WriteLine("Reflection Distance: " + reflection.Distance);

            // Enregistrez le classeur
            workbook.Save("ReflectionEffectDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


