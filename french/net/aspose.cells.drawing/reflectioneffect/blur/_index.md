---
title: "ReflectionEffect.Blur"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ReflectionEffect property. Obtient et définit le rayon du flou en unité de points"
type: docs
url: /fr/net/aspose.cells.drawing/reflectioneffect/blur/
---
## ReflectionEffect.Blur property

Obtient et définit le rayon du flou,in unités de points.

```csharp
public double Blur { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ReflectionEffectPropertyBlurDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une forme rectangulaire
            Aspose.Cells.Drawing.Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            
            // Accédez à l'effet de réflexion
            Aspose.Cells.Drawing.ReflectionEffect reflection = rectangle.Reflection;
            
            // Définissez le type de réflexion et les propriétés
            reflection.Type = Aspose.Cells.Drawing.ReflectionEffectType.HalfReflectionTouching;
            reflection.Blur = 0.5; // Demonstrate Blur property
            reflection.Transparency = 0.5;
            reflection.Size = 55;
            reflection.Distance = 0;
            
            // Enregistrez le classeur
            workbook.Save("ReflectionEffectDemo.xlsx");
            
            // Affichez la valeur du flou
            Console.WriteLine("Reflection Blur: " + reflection.Blur);
        }
    }
}
```

### Voir aussi

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


