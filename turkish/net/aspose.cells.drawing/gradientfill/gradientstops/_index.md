---
title: "GradientFill.GradientStops"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GradientFill özelliği. Degrade durakları koleksiyonunu temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/gradientfill/gradientstops/
---
## GradientFill.GradientStops property

Gradyan durak noktası koleksiyonunu temsil eder.

```csharp
public GradientStopCollection GradientStops { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class GradientFillPropertyGradientStopsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;
            
            // Bir dikdörtgen şekli ekle
            Shape shape = shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            // Degrade dolgu ayarla
            shape.Fill.FillType = FillType.Gradient;
            GradientFill gradientFill = shape.Fill.GradientFill;
            
            // Mevcut tüm degrade duraklarını temizle
            gradientFill.GradientStops.Clear();

            // Özel degrade durakları ekle
            gradientFill.GradientStops.Add(0.0, Color.Red, 255);
            gradientFill.GradientStops.Add(0.5, Color.Yellow, 255);
            gradientFill.GradientStops.Add(1.0, Color.Green, 255);

            // Degrade duraklarına erişimi göster
            Console.WriteLine("Gradient Stops Count: " + gradientFill.GradientStops.Count);
            Console.WriteLine("First Stop Position: " + gradientFill.GradientStops[0].Position);
            Console.WriteLine("Second Stop Color: " + gradientFill.GradientStops[1].CellsColor);

            workbook.Save("GradientFillDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [GradientStopCollection](../../gradientstopcollection/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


