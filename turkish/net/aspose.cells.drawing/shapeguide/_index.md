---
title: "Sınıf ShapeGuide"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.ShapeGuide sınıfı. Bir şekil kılavuzunu kapsar ve belirtilen şeklin geometrisini yönetecek bir şekil kılavuzunun varlığını belirtir."
type: docs
url: /tr/net/aspose.cells.drawing/shapeguide/
---
## ShapeGuide class

Bir şekil kılavuzunun varlığını belirten ve belirtilen şeklin geometrisini yönetecek bir şekil kılavuzunu kapsüller.

```csharp
public class ShapeGuide : BaseShapeGuide
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Value](../../aspose.cells.drawing/shapeguide/value/) { get; set; } | Bu kılavuzun değerini alır veya ayarlar |

### Örnekler

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
                
                // Gerekli parametrelerle şekil kılavuzu oluştur ve ekle
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

### Ayrıca Bakınız

* class [BaseShapeGuide](../baseshapeguide/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


