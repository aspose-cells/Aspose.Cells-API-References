---
title: "ReflectionEffect.Direction"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ReflectionEffect. Obtient et définit la direction du dégradé alpha par rapport à la forme elle-même"
type: docs
url: /fr/net/aspose.cells.drawing/reflectioneffect/direction/
---
## ReflectionEffect.Direction property

Obtient et définit la direction de la rampe de dégradé alpha par rapport à la forme elle-même.

```csharp
public double Direction { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ReflectionEffectPropertyDirectionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme pour appliquer l'effet de réflexion
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
            
            // Obtenir l'effet de réflexion de la forme
            ReflectionEffect reflection = shape.Reflection;
            
            // Afficher la valeur actuelle de Direction
            Console.WriteLine("Current Direction value: " + reflection.Direction);
            
            // Définir une nouvelle valeur Direction (90 degrés)
            reflection.Direction = 90;
            Console.WriteLine("New Direction value: " + reflection.Direction);
            
            // Configurer d'autres propriétés de réflexion pour une meilleure visibilité
            reflection.Type = ReflectionEffectType.TightReflectionTouching;
            reflection.Transparency = 0.5;
            reflection.Size = 50;
            reflection.Blur = 5;
            
            // Enregistrer le classeur pour voir l'effet de réflexion
            workbook.Save("ReflectionEffectDirectionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


