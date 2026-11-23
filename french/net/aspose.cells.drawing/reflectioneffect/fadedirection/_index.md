---
title: "ReflectionEffect.FadeDirection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ReflectionEffect. Obtient et définit la direction pour décaler la réflexion"
type: docs
url: /fr/net/aspose.cells.drawing/reflectioneffect/fadedirection/
---
## ReflectionEffect.FadeDirection property

Obtient et définit la direction du décalage de la réflexion.

```csharp
public double FadeDirection { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ReflectionEffectPropertyFadeDirectionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme pour appliquer l'effet de réflexion
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            // Obtenir l'effet de réflexion de la forme
            ReflectionEffect reflection = shape.Reflection;

            // Afficher la valeur actuelle de FadeDirection
            Console.WriteLine("Current FadeDirection value: " + reflection.FadeDirection);

            // Définir une nouvelle valeur FadeDirection (90 degrés)
            reflection.FadeDirection = 90;
            Console.WriteLine("New FadeDirection value: " + reflection.FadeDirection);

            // Configurer d'autres propriétés de réflexion pour une meilleure visibilité
            reflection.Type = ReflectionEffectType.TightReflectionTouching;
            reflection.Transparency = 0.5;
            reflection.Size = 50;
            reflection.Blur = 5;
            reflection.Distance = 10;

            // Enregistrer le classeur pour voir l'effet
            workbook.Save("ReflectionEffectFadeDirectionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


