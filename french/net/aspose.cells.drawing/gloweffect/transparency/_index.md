---
title: "GlowEffect.Transparency"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété GlowEffect. Obtient et définit le degré de transparence de l'effet de lueur. Plage de 0.0 opaque à 1.0 clair"
type: docs
url: /fr/net/aspose.cells.drawing/gloweffect/transparency/
---
## GlowEffect.Transparency property

Obtient et définit le degré de transparence de l'effet de lueur. Plage de 0,0 (opaque) à 1,0 (transparent).

```csharp
public double Transparency { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class GlowEffectPropertyTransparencyDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            Shape shape = sheet.Shapes.AddAutoShape(AutoShapeType.RoundedRectangle, 0, 10, 0, 10, 200, 100);
            shape.Glow.Size = 8;
            shape.Glow.Transparency = 0.6;
            
            CellsColor glowColor = shape.Glow.Color;
            glowColor.ThemeColor = new ThemeColor(ThemeColorType.Accent2, 0);

            wb.Save("output/glow_transparency_demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [GlowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


