---
title: "GradientFill.FillType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GradientFill özelliği. Gradyan doldurma tipini alır"
type: docs
url: /tr/net/aspose.cells.drawing/gradientfill/filltype/
---
## GradientFill.FillType property

Degrade dolgu türünü alır.

```csharp
public GradientFillType FillType { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class GradientFillPropertyFillTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gradyan doldurma ile bir şekil oluştur
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            FillFormat fillFormat = shape.Fill;
            fillFormat.FillType = FillType.Gradient;
            
            // Gradyan özelliklerini ayarla
            GradientFill gradientFill = fillFormat.GradientFill;
            gradientFill.SetTwoColorGradient(System.Drawing.Color.Red, System.Drawing.Color.Blue, GradientStyleType.Horizontal, 1);
            
            // Gradyan doldurma tipini görüntüle
            Console.WriteLine("Gradient Fill Type: " + gradientFill.FillType);
            
            // Dairesel gradyana değiştir
            gradientFill.SetGradient(GradientFillType.Radial, 45, GradientDirectionType.FromCenter);
            Console.WriteLine("Updated Gradient Fill Type: " + gradientFill.FillType);
            
            // Çalışma kitabını kaydedin
            workbook.Save("GradientFillDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [GradientFillType](../../gradientfilltype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


