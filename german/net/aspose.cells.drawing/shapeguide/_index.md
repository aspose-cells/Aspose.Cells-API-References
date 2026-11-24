---
title: "Klasse ShapeGuide"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.ShapeGuide Klasse. Kapselt einen Formleitfaden, der das Vorhandensein eines Formleitfadens angibt, der zur Steuerung der Geometrie der angegebenen Form verwendet wird."
type: docs
url: /de/net/aspose.cells.drawing/shapeguide/
---
## ShapeGuide class

Kapselt einen Shape-Guide, der das Vorhandensein eines Shape-Guides angibt, der verwendet wird, um die Geometrie der angegebenen Form zu steuern

```csharp
public class ShapeGuide : BaseShapeGuide
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Value](../../aspose.cells.drawing/shapeguide/value/) { get; set; } | Liest oder setzt den Wert dieses Leitfadens |

### Beispiele

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
                
                // Formleitfaden mit erforderlichen Parametern erstellen und hinzufügen
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

### Siehe auch

* class [BaseShapeGuide](../baseshapeguide/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


