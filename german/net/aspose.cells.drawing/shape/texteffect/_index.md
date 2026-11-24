---
title: "Shape.TextEffect"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt ein TextEffectFormat-Objekt zurück, das TextEffect-Formatierungseigenschaften für die angegebene Form enthält. Gilt für Shape-Objekte, die WordArt darstellen."
type: docs
url: /de/net/aspose.cells.drawing/shape/texteffect/
---
## Shape.TextEffect property

Gibt ein TextEffectFormat-Objekt zurück, das Text‑Effekt‑Formatierungseigenschaften für die angegebene Form enthält. Gilt für Shape-Objekte, die WordArt darstellen.

```csharp
public TextEffectFormat TextEffect { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextEffectDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie eine WordArt-Form mit den richtigen Parametern hinzu.
            Shape shape = worksheet.Shapes.AddWordArt(PresetWordArtStyle.WordArtStyle1, "Sample Text", 10, 10, 200, 50, 0, 0);

            // Prüfen Sie, ob es sich um WordArt handelt, und greifen Sie auf TextEffect-Eigenschaften zu.
            if (shape.IsWordArt)
            {
                TextEffectFormat textEffectFormat = shape.TextEffect;
                textEffectFormat.FontBold = true;
                textEffectFormat.FontItalic = true;
                textEffectFormat.FontName = "Arial";
                textEffectFormat.FontSize = 14;
            }

            // Speichere die Arbeitsmappe
            workbook.Save("TextEffectDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextEffectFormat](../../texteffectformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


