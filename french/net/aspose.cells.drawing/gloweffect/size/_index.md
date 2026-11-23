---
title: "GlowEffect.Size"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété GlowEffect. Obtient et définit le rayon de la lueur en unités de points"
type: docs
url: /fr/net/aspose.cells.drawing/gloweffect/size/
---
## GlowEffect.Size property

Obtient et définit le rayon de la lueur, en unité de points.

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
    public class GlowEffectPropertySizeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.RoundedRectangle, 10, 10, 200, 100, 200, 100);
            
            // Définir les propriétés de l'effet de lueur
            shape.Glow.Size = 8;
            shape.Glow.Transparency = 0.6;
            shape.Glow.Color.ThemeColor = new ThemeColor(ThemeColorType.Accent2, 0);

            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [GlowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


