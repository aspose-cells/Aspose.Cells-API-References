---
title: "Classe ShapeGuide"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.ShapeGuide. Encapsule un guide de forme qui spécifie la présence d'un guide de forme qui sera utilisé pour gouverner la géométrie de la forme spécifiée"
type: docs
url: /fr/net/aspose.cells.drawing/shapeguide/
---
## ShapeGuide class

Encapsule un guide de forme qui spécifie la présence d'un guide de forme qui sera utilisé pour gouverner la géométrie de la forme spécifiée

```csharp
public class ShapeGuide : BaseShapeGuide
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Value](../../aspose.cells.drawing/shapeguide/value/) { get; set; } | Obtient ou définit la valeur de ce guide |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapeGuideDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                var shape = worksheet.Shapes.AddAutoShape(AutoShapeType.RoundedRectangle, 0, 0, 100, 100, 100, 100);
                
                // Créer et ajouter un guide de forme avec les paramètres requis
                int guideIndex = shape.Geometry.ShapeAdjustValues.Add("Guide1", 0.2);
                ShapeGuide guide = shape.Geometry.ShapeAdjustValues[guideIndex];
                
                Console.WriteLine($"ShapeGuide created with Value: {guide.Value}");
                
                workbook.Save("DrawingClassShapeGuideDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [BaseShapeGuide](../baseshapeguide/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


