---
title: "PatternFill.BackTransparency"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PatternFill özelliği. Arka plan renginin şeffaflığını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/patternfill/backtransparency/
---
## PatternFill.BackTransparency property

Arka plan renginin şeffaflığını alır veya ayarlar.

```csharp
public double BackTransparency { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class PatternFillPropertyBackTransparencyDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir dikdörtgen şekli ekle
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 200, 200);

            // Şekilden mevcut PatternFill örneğini alın ve özellikleri yapılandırın
            shape.Fill.FillType = FillType.Pattern;
            PatternFill patternFill = shape.Fill.PatternFill;
            patternFill.Pattern = FillPattern.Solid;
            patternFill.BackgroundColor = Color.Blue;

            // İlk BackTransparency değerini gösterin
            Console.WriteLine("Current BackTransparency value: " + patternFill.BackTransparency);

            // Yeni BackTransparency değerini ayarlayın (%50 şeffaflık)
            patternFill.BackTransparency = 0.5;

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("PatternFillBackTransparencyDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


