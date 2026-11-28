---
title: "Enum GradientFillType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.GradientFillType enum. Tüm Gradient dolgu türlerini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/gradientfilltype/
---
## GradientFillType enumeration

Tüm Degrade doldurma tipini temsil eder.

```csharp
public enum GradientFillType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Linear | `0` | Doğrusal |
| Radial | `1` | Radyal |
| Rectangle | `2` | Dikdörtgen |
| Path | `3` | Yol |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassGradientFillTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gradient dolgu göstermek için bir şekil oluştur
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 5, 5, 20);

            // Dolgu formatını al
            FillFormat fillFormat = shape.Fill;

            // Gradient dolgu türünü ve özelliklerini ayarla
            fillFormat.SetTwoColorGradient(System.Drawing.Color.Blue, System.Drawing.Color.LightBlue, GradientStyleType.Horizontal, 1);
            fillFormat.GradientFill.SetGradient(GradientFillType.Linear, 45, GradientDirectionType.FromUpperLeftCorner);

            // Gradient yön türünü çıktı olarak ver
            Console.WriteLine("Gradient Direction Type: " + fillFormat.GradientFill.DirectionType);

            // Çalışma kitabını kaydedin
            workbook.Save("GradientFillTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


