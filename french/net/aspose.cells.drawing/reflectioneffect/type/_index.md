---
title: "ReflectionEffect.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ReflectionEffect property. Obtient et définit l'effet de réflexion prédéfini"
type: docs
url: /fr/net/aspose.cells.drawing/reflectioneffect/type/
---
## ReflectionEffect.Type property

Obtient et définit l'effet de réflexion prédéfini.

```csharp
public ReflectionEffectType Type { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ReflectionEffectPropertyTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une forme rectangulaire
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            
            // Obtenez l'effet de réflexion
            ReflectionEffect reflection = shape.Reflection;
            
            // Démontrez la propriété Type
            Console.WriteLine("Initial reflection type: " + reflection.Type);
            
            // Changez le type de réflexion
            reflection.Type = ReflectionEffectType.HalfReflectionTouching;
            Console.WriteLine("Updated reflection type: " + reflection.Type);
            
            // Définissez d'autres propriétés de réflexion
            reflection.Transparency = 0.5;
            reflection.Size = 55;
            reflection.Blur = 0.5;
            reflection.Distance = 0;
            
            // Enregistrez le classeur
            workbook.Save("ReflectionEffectDemo.xlsx");
            
            Console.WriteLine("Demo completed successfully.");
        }
    }
}
```

### Voir aussi

* enum [ReflectionEffectType](../../reflectioneffecttype/)
* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


