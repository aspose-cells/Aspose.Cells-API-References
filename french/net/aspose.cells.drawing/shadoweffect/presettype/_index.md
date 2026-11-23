---
title: "ShadowEffect.PresetType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ShadowEffect. Obtient et définit le type d’ombre prédéfini de l’ombre"
type: docs
url: /fr/net/aspose.cells.drawing/shadoweffect/presettype/
---
## ShadowEffect.PresetType property

Obtient et définit le type d'ombre prédéfini de l'ombre.

```csharp
public PresetShadowType PresetType { get; set; }
```

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShadowEffectPropertyPresetTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            ShadowEffect shadow = shape.ShadowEffect;
            
            shadow.PresetType = PresetShadowType.OffsetBottom;
            shadow.Color = workbook.CreateCellsColor();
            shadow.Color.Color = Color.Blue;
            shadow.Transparency = 0.3;
            shadow.Size = 80;
            shadow.Blur = 20;
            shadow.Distance = 6;

            workbook.Save("ShadowEffectDemo.xlsx");

            Workbook loadedWorkbook = new Workbook("ShadowEffectDemo.xlsx");
            ShadowEffect loadedShadow = loadedWorkbook.Worksheets[0].Shapes[0].ShadowEffect;
            
            Console.WriteLine("PresetType: " + loadedShadow.PresetType);
            Console.WriteLine("Transparency: " + loadedShadow.Transparency);
        }
    }
}
```

### Voir aussi

* enum [PresetShadowType](../../presetshadowtype/)
* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


