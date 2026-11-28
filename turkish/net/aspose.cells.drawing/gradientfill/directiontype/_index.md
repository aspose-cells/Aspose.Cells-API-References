---
title: "GradientFill.DirectionType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GradientFill özelliği. Gradyan yön tipini alır"
type: docs
url: /tr/net/aspose.cells.drawing/gradientfill/directiontype/
---
## GradientFill.DirectionType property

Degrade yön türünü alır.

```csharp
public GradientDirectionType DirectionType { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class GradientFillPropertyDirectionTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gradient dolgu göstermek için bir şekil oluştur
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 5, 5, 5);

            // Gradyan dolgu özelliklerini ayarla
            FillFormat fillFormat = shape.Fill;
            fillFormat.SetTwoColorGradient(System.Drawing.Color.Blue, System.Drawing.Color.LightBlue, GradientStyleType.DiagonalDown, 1);
            fillFormat.GradientFill.SetGradient(GradientFillType.Linear, 45, GradientDirectionType.FromUpperLeftCorner);

            // Gradyan yön türünü çıktıya gönder
            Console.WriteLine("Gradient Direction Type: " + fillFormat.GradientFill.DirectionType);

            // Çalışma kitabını kaydedin
            workbook.Save("GradientDirectionTypeExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [GradientDirectionType](../../gradientdirectiontype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


